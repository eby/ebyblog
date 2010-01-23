--- 
wordpress_id: 612
layout: post
title: Unicode and Sphinx
wordpress_url: http://blog.ryaneby.com/?p=612
---
I'm not an expert with unicode and ran into various problems in getting Sphinx up and running with bib data for <a href="http://thesocialopac.net/">SOPAC2</a>. Below is an overview of what I ended up doing to solve it. There are probably better ways of doing it and if so please share.

The Sphinx I'm referring to is <a href="http://www.sphinxsearch.com/">the indexing/search program</a> that works well with MySQL. The case below is using the stock searchd/indexer interface and not the mysql engine which is probably different.

<h4>Convert to UTF8 in MySQL</h4>

You can convert tables and all the fields within the table with the command (from <a href="http://wolfram.kriesing.de/blog/index.php/2007/convert-mysql-db-to-utf8">pythoneer</a>):

{% highlight mysql %}
ALTER TABLE tbl_name CONVERT TO CHARACTER SET utf8 COLLATE utf8_unicode_ci;
{% endhighlight %}

You could also do utf8_general_ci. From what I've picked up online is that the unicode_ci supports expansions/ligatures while the general doesn't which can affect sorting. However, the docs say the <a href="http://dev.mysql.com/doc/refman/5.0/en/charset-unicode-sets.html">the tradeoff is speed</a> in some operations. Both lack some character support versus the actual Unicode Collation Algorithm.

<h4>Configure Sphinx for Unicode</h4>

You will want to set your index definition to have:

{% highlight mysql %}
charset_type = utf-8
{% endhighlight %}

While the docs mostly just mention that I highly recommend adding the following to your source definition:

{% highlight mysql %}
sql_query_pre = SET CHARACTER_SET_RESULTS=utf8
sql_query_pre = SET NAMES utf8
{% endhighlight %}

While you might think that having your tables in utf8 collation, mysql set to default to it and php encoding in utf8 would be enough, if the client doesn't specify that it is doing utf8 mysql will store it in whatever encoding it thinks it is getting. I battled with php configs to try to ensure all machines modifying the tables were talking the same but you'll save yourself the trouble by defining this here and also in your scripts that write to the tables.

<h4>Modify your insertions to SET NAMES</h4>

As stated above I'd recommend doing a SET NAMES utf8 in front of your queries inserting data into mysql. This again may be poor setup on my part but it helps rule out different client configurations and probably makes it more portable. I found Gentoo by default seems to do fine, Debian hit or miss. Adding the SET made it work where ever I tried.

Some documentation stated I should wipe database if it previously had other encodings. I found this unnecessary and just inserted the data with UPDATE or REPLACE INTO and had no issues.

<h4>Set up character folding</h4>

While stop words and similar allow you to use external files for the list, it appears character folding needs the list to be in the config itself. At least I haven't been able to get an include file to work. I'd be interested in knowing otherwise. Depending on the languages you have you may want to generate a list of the codes present in your dataset. Otherwise you can find some tables to try out here:

<ul>
<li><a href="http://yob.id.au/2008/05/08/thinking-sphinx-and-unicode.html">Thinking Sphinx And Unicode</a></li>
<li><a href="http://speeple.com/unicode-maps.txt">Unicode Map at Speeple.com</a></li>
</ul>

Some reported that Sphinx can have issues with long lines in the config so you may need to break up the lines with \ characters. Your list should also include "0..9, a..z, A..Z->a..z" in it as you are overriding the default list.

<h4>Reindex</h4>

Another thing to note with Sphinx is that many changes to the sphinx.conf requires a restart of searchd. With the modification of the folding table you'll probably want to do this. Restart searchd and then do your indexer run for your indexes.

 Try out some searches with keywords/characters and watch the query log. If the character folding is working then you should see the encoded characters in the query log. If they are missing or replaced by spaces then the characters aren't matching up with your folding table. Try to find the character, add it to your list, restart searchd and reindex. Sphinx defaults to not accepting characters that are not in the charset_table list. The query log is the easiest point to diagnose this at.

<h4>Web Display</h4>

The last step is of course to make sure your web pages are served in a proper encoding so browsers render it properly.

Again this isn't in depth but hopefully will help those messing with Sphinx.
