--- 
wordpress_id: 201
layout: post
title: Searching OpenWorldCat
wordpress_url: http://blog.ryaneby.com/archives/searching-openworldcat/
---
<a href="http://babyboomerlibrarian.blogspot.com/2006/03/value-of-openworldcat.html">Bill Drew posts about his doubts with OpenWorldCat</a>. During code4lib2006 I got the chance to drink and complain with Eric Hellman of <a href="http://openly.com/">Openly</a>/OCLC. Since I'm more of a patron most of my complaints were about OpenWorldCat. One of my criticisms was that it was so hard to search. If you go to <a href="http://www.oclc.org/worldcat/open/default.htm">worldcatlibraries.org</a> then you get a nice vendor page for the product. If you go to <a href="http://worldcat.org/">worldcat.org</a> you get a login screen. As far as I know there is no easy to remember site that I can plug into my browser and easily search OpenWorldCat. Once your on a record within it you can easily search and they do have a <a href="http://www.oclc.org/worldcat/open/tryit/default.htm">"demo" page</a> but that's not the easiest to find.

I'd really like to see the demo page cleaned up a bit and put at some memorable url. OCLC has been steadily improving so this may be in the works. It is possible, however, for your library to include a simple search box in a page that will fire off a search to a search engine and limit to OpenWorldCat results. Your probably asking yourself what value this has when the person is already on your library site. The first is that it advertises the service which the patron may find useful in the future if they are trying to find a book you don't have or a specific edition. It's also helpful for those who may have some problems searching the OPAC. OpenWorldCat doesn't have your entire catalog most likely but it could be the thing that prevents them from giving up and going to Amazon.

Since both Yahoo and Google have search API's there is the option of actually including the results into your own applications. I'd like to see OCLC offer some API's of their own if they don't already. But to keep things simple I'll just show you how to create a simple search box that limits results.

<h3>Form to search Google Scholar</h3>

<code>
&lt;form action="http://www.google.com/scholar" name="f"&gt;<br />
&lt;input maxlength="256" size="40" name="q" value="" /&gt;<br />
&lt;input type="hidden" name="ie" value="UTF-8" /&gt;<br />
&lt;input type="hidden" name="oe" value="UTF-8" /&gt;<br />
&lt;input type="hidden" name="hl" value="en" /&gt;<br />
&lt;input type="hidden" name="domains" value="worldcatlibraries.org" /&gt;<br />
&lt;input type="hidden" name="sitesearch" value="worldcatlibraries.org" /&gt;<br />
&lt;input type="submit" value="Search Google Scholar" name="btnG" /&gt;<br />
&lt;/form&gt;
</code>

<h3>Form to search Google</h3>

<code>
&lt;form action="http://www.google.com/search" name="f"&gt;<br />
&lt;input maxlength="256" size="40" name="q" value="" /&gt;<br />
&lt;input type="hidden" name="ie" value="UTF-8" /&gt;<br />
&lt;input type="hidden" name="oe" value="UTF-8" /&gt;<br />
&lt;input type="hidden" name="hl" value="en" /&gt;<br />
&lt;input type="hidden" name="domains" value="worldcatlibraries.org"&gt;<br />
&lt;input type="hidden" name="sitesearch" value="worldcatlibraries.org" /&gt;<br />
&lt;input type="submit" value="Search Google" name="btnG" /&gt;<br />
&lt;/form&gt;
</code>

Hope this is helpful to someone.
