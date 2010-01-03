--- 
wordpress_id: 271
layout: post
title: SRU Interface for the III XML Server
wordpress_url: http://blog.ryaneby.com/archives/sru-interface-for-the-iii-xml-server/
---
I may be giving a presentation at the summer <a href="http://www.miug.org/">MIUG</a> meeting regarding uses of the III XML Server. Regardless if that ends up occurring I figure I should post some of the applications here. I'm sure it will help the presentation as well if people fix all my mistakes ;-) The first of these is the <a href="http://public.csusm.edu/dwalker/shrew/">Shrew project</a> by <a href="http://public.csusm.edu/dwalker/">David Walker</a> of Cal State San Marcos.

<h4>Shrew</h4>

Shrew itself is a SRU server that lays on top of the III XML Server and allows you standardized access to the III OPAC. For an idea here is a simple diagram:

<a href="http://www.flickr.com/photos/ebyryan/155576658/" title="Photo Sharing"><img src="http://static.flickr.com/70/155576658_822ec5ee93.jpg" width="500" height="116" alt="shrew diagram" /></a>

You may think this is a needless layer. Why not just build the interface on top of the XML Server itself. Here are a few reasons:

<ul>
<li>Standardized. By using a non-proprietary structure it makes it easier to integrate the III software with other products that may already support it. An example is below. SRU/MarcXML is starting to be used more widely.</li>
<li>Abstraction. When something changes with the III server (and it likely will), all you have to do is change the Shrew library. Those applications that are built on top of it should not have to be changed. One point of failure.</li>
</ul>

Here are some links that should get you going:

<ul>
<li><a href="http://library.csusm.edu/catalog/sru/">Shrew</a> - This is the actual SRU interface. The Explain document has been changed to a form with XSL.</li>
<li><a href="http://library.csusm.edu/catalog/sru/example/">Example Interface</a> - Here is an example interface built directly on Shrew. Basic with some Amazon integration. Not all features work but should give you an idea.</li>
</ul>

<h4>Meta-Search</h4>

For a better example of the usefulness of this, let's take a look at a more elaborate example. One of David's uses of Shrew is to integrate the III holdings with a metasearch product. They have decided to look at MetaLib by Ex Libris which can consume SRU-based servers and has an XML-based product that allows custom interfaces to be built on top of it. This means the III server becomes another holding source like any other that can be included in results. Here is a brief diagram:

<a href="http://www.flickr.com/photos/ebyryan/155576657/" title="Photo Sharing"><img src="http://static.flickr.com/57/155576657_4ec1232517.jpg" width="500" height="321" alt="metalib xserver and innopac" /></a>

There are <a href="http://public.csusm.edu/dwalker/xerxes/">some articles up on David Walker's site regarding this project (codename Xerxes)</a>. The interface is currently under development and isn't public but here are some screenshots to give you an idea of what's possible. As far as I know this is far from the final interface so don't get too attached ;-)

Here is the search screen for the Biology Topic area:

<a href="http://www.flickr.com/photos/ebyryan/155602703/" title="Photo Sharing"><img src="http://static.flickr.com/74/155602703_093dd4f939.jpg" width="500" height="317" alt="metasearch for topic" /></a>

Here is the results screen for a search. You can see the book holdings mixed in with the other results:

<a href="http://www.flickr.com/photos/ebyryan/155602704/" title="Photo Sharing"><img src="http://static.flickr.com/74/155602704_42f340bb81.jpg" width="500" height="311" alt="metasearch results" /></a>

As you can probably tell abstracting the III opac under a SRU layer can make things easier and open quite a few possibilities with integration. As SRU becomes more popular the possibilities will grow.
