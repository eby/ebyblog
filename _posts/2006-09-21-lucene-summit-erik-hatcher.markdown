--- 
wordpress_id: 368
layout: post
title: "Lucene Summit: Erik Hatcher"
wordpress_url: http://blog.ryaneby.com/archives/lucene-summit-erik-hatcher/
---
The co-author of Lucene in Action, this presentation could probably have been termed a keynote. Erik is working with Lucene and Solr in quite a few projects and some of the displays are fairly interesting. Most of these projects are listed under <a href="http://patacriticism.org/projects.html">patacriticism.org</a> though there is another called <a href="http://www.patacriticism.org/juxta/">Juxta</a> which also used Lucene though mostly for data analysis.

<h4>Rosetti Archive</h4>
<ul>
<li>Available at <a href="http://www.rossettiarchive.org/">rossettiarchive.org</a></li>
<li>Uses lucene for full text search</li>
<li>Has multiple types of digitized objects - poems, paintings, etc</li>
<li>Scholars demanded case sensitive version - accomplished with two seperate indexes - checkbox chooses index</li>
<li>Metadata is mixed - some have alot, some don't, many based on crappy xml formats</li>
<li>More like this function that creates query from object data</li>
</ul>

<h4>Nines and Collex</h4>
<ul>
<li>A scholary portal for 19th century objects.</li>
<li>Available at <a href="http://www.nines.org/collex">www.nines.org/collex</a></li>
<li>Interface uses idea of facets/sets/collections - add and subtract facets to limit your collection - keyword not really necessary</li>
<li>facets are intersections between sets</li>
<li>objects can be in multiple sets</li>
<li>counts shown are specific to the current restraints - dynamic - cached to speed up</li>
<li>can intercept any set - example: everything in a category i haven't collected/taged</li>
<li>username, collection - just another facet - everything is a set - sets can be objects</li>
<li>there is an index for the archive and a seperate index for user data currently</li>
<li>docsets used for users</li>
<li>currently writing an update handler for solr to help make dynamic/user data easier to handle - update single fields</li>
<li>hopeful to allow member archives to use the connections users make within collex</li>
<li>atom exports one possibility</li>
<li>open-source project at sourceforge but not really general at this point</li>
<li>ruby on rails frontend with solr on the backend. mysql is also used for some user data, may contain index in future</li>
<li>rdf -> solr right now. member archives submit the rdf format or are converted to it</li>
<li>future: move more things to mysql so displays can be built faster without pulling information from index itself (limit lucene/solr for searching)</li>
</ul>

There was more information in the presentation but I found it hard to summarize some of it. I really found the Collex interface concept to be very interesting. Everything is a contraint or limit and you can easily add or invert the contraint. It's also easy to add things to a personal collection and parts of the personal collection then become facets/contraints themselves. He's really using all of the metadata (archive and user) to it's full extent. He also has more plans including "exhibits" where people can "curate collections". These collections themselves can then become objects in the index and so on. This project will be something to watch.
