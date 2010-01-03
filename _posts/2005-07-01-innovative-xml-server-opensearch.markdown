--- 
wordpress_id: 26
layout: post
title: Innovative XML Server - OpenSearch
excerpt: I've been working on various ideas for using our Innovative XML server. I first began with creating html views of featured lists. Once I had the syntax down I created RSS 2.0 feeds for the lists. While I was doing this I came across a <a href="http://open-ils.org/blog/?p=29">post over at open-ils</a> that referred to OpenSearch. I had done a little with OpenSearch when it first came out but not since I started playing with the XML server. BTW, I recommend reading the whole post over at open-ils. Lots of great thinking in it.
wordpress_url: http://ebybox.aresgate.net/blog/?p=26
---
I've been working on various ideas for using our Innovative XML server. I first began with creating html views of featured lists. Once I had the syntax down I created RSS 2.0 feeds for the lists. While I was doing this I came across a <a href="http://open-ils.org/blog/?p=29">post over at open-ils</a> that referred to OpenSearch. I had done a little with <a href="http://opensearch.a9.com/">OpenSearch</a> when it first came out but not since I started playing with the XML server. BTW, I recommend reading the whole post over at open-ils. Lots of great thinking in it.

So here's the end product:
<a href="http://a9.com/harry%20potter?a=sB0007WF86M">http://a9.com/harry%20potter?a=sB0007WF86M</a>

You'll notice that right now I only have the title and availabilities. This is because it was a quick mock-up and I wanted to make things a bit quicker (why in a future post). You can really add any data from the XML output by modifying the XSL file for the description. I find this is really easy to read though I really should add the pub date and call number. A special note as well: certain resources didn't seem to have a call number (thesis I think) so I chose to link to the OPAC by bib number. This also is a time saver as it is returned in the basic XML result.

<h4>How to do it</h4>

First you'll need something server-side that can transform xml. I prefer to use php5 as these things are really simple in it. What you'll do is take arguments on the URL and then create a xml server query using it. For example here is a sample OpenSearch URL:

<code>opensearch.php?q=harry%20potter&amp;p=1&amp;c=10</code>

This sets the query to be "harry potter", the first page of results and 10 titles returned. The resulting xml server query would be:

<code>path.to.xmlopac/.$term."/0/0/".$page."/".$count."?avsrank=D&amp;noexclude=WXROOT.Heading.Title.IIIRECORD&amp;exclude=WXROOT.Heading.Title.IIIRECORD.VARFLDPRIMARYALTERNATEPAIR</code>

A quick runthrough of what I'm doing. The $term is actually the query from the URL with a "X" put in front of it to signify that it is keyword. I could just put the X right in the url line but remember I'm reusing this from my RSS work which actually allows you to choose what kind of search. Page and count are simlar except where I have page is actually the result number. I do some arithmetic behind the scenes so page 2 starts at result 11. I know this is confusing and opensearch supports passing result number but again with was something I reused from before.

Once you have the URL you will want to apply XSLT to it. Here's the full template to transform your XML result into OpenSearch:

<a href="http://ebybox.aresgate.net/blog/stuff/opensearch.xsl">XSL File</a> (you may need to view source as I don't have all my mimetypes set)

You then need to make your script return the resulting feed. In my case I just echo'd the result. There's an additional file you need to create to describe your opensearch interface which is outlined at the OpenSearch site. My explanation is probably bad so here are the 3 files you need:

<ul>
<li><a href="http://ebybox.aresgate.net/blog/stuff/opensearch.phps">opensearch.php</a></li>
<li><a href="http://ebybox.aresgate.net/blog/stuff/opensearch.xml">opensearch.xml</a> - definition</li>
<li><a href="http://ebybox.aresgate.net/blog/stuff/opensearch.xsl">opensearch.xsl</a></li>
</ul>

I'm learning as I go so feel free to offer suggestions on coding, but please don't mock.
