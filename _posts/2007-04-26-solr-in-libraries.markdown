--- 
wordpress_id: 513
layout: post
title: Solr in Libraries
wordpress_url: http://blog.ryaneby.com/archives/solr-in-libraries/
---
Note: Many of the examples below only include screenshots. As these are development versions I don't want to overwhelm them with traffic. If you pop in #code4lib you'll probably be able to get a peek at them.

h3. What is Solr?

If you were at Code4Lib 2007 then you were probably beat over the head with Solr. If not then here is a very brief intro. Solr is currently an incubator project of the Apache Foundation, part of the Lucene project. The brief intro from "their site":http://lucene.apache.org/solr/:

bq. Solr is an open source enterprise search server based on the Lucene Java search library, with XML/HTTP and JSON APIs, hit highlighting, faceted search, caching, replication, and a web administration interface. It runs in a Java servlet container such as Tomcat.

While that sums it up, it really doesn't tell you how truly useful it is. To begin with Lucene is a powerful full-text search engine. Solr builds on top of Lucene to add a plethora of features that make building search-centric applications much easier. Many of the projects I feature below are one-person spare-time projects which likely would have been more difficult to accomplish without Solr. Some of the features Solr provides:

* Ability to do all operations, including submitting new documents, over HTTP requests (GET and POST)
* XML data format (both input and output), making it easy to parse in many programming languages
* Ability to easily index a single field in multiple ways
* Hilighting of search terms in results
* Faceting of results
* Query-time boosting, meaning multiple interfaces with different results can be built on same index
* Lots of caching and replication features

Some of the "people who use it outside of libraries":http://wiki.apache.org/solr/PublicServers include CNET and the Internet Archive.

h3. A Live Example

To start off with a non-library example, here is some information about "Internet Archive's":http://archive.org/ change "to solr":http://www.nabble.com/INTERNET-ARCHIVE-goes-SOLR!-tf3129097.html

After two days with Solr they averaged about 5.4 queries per second on an index of approximately 575k+ items. Even with this type of load they were able to do it with a single 4GB RAM dual core machine (instead of the 3 they used before). They also averaged a 0.5 load with sar showing 80% resources idle.

As for their index they updated it every 15 minutes and didn't really optimize it other then the schema. Most of the Solr install was stock and they even did their boosting on query-time. An example of their query parsing "is given in the email announcement":http://www.nabble.com/INTERNET-ARCHIVE-goes-SOLR!-tf3129097.html

h1. Some Library Examples

h3. David Walker's Solr Experiment

<a href="http://www.flickr.com/photos/ebyryan/473822142/" title="Photo Sharing"><img src="http://farm1.static.flickr.com/199/473822142_a1ee4546be.jpg" width="500" height="378" alt="Walker's Solr Search" /></a>

Walker, "who has been working on many things":http://public.csusm.edu/dwalker/, threw together a Solr catalog built on Innovative Interfaces data exports. Specifically he took tab-delimited data exports and imported them into Solr. He then wrote a PHP5-based interface to his Solr instance. While proof-of-concept right now there is hope that it might become something and possibly experiment with union catalog interfaces.

He also used Amazon data for the images and some review information on the item record page. One of the things that caught my eye was the item record view itself:

<a href="http://www.flickr.com/photos/ebyryan/473823462/" title="Photo Sharing"><img src="http://farm1.static.flickr.com/183/473823462_e888e85591.jpg" width="500" height="374" alt="Walker's Solr Record View" /></a>

One of the challenges is getting live status information into the catalog. An easy solution is to just link to the vendor supplied catalog for the item pages. The solution here is to actually scrape the MARC view of the III catalog which supplies both the item information and it III's case, the status info. This is then parsed to allow custom layouts to be created. The example above includes some Amazon data in addition to the normal stuff.

h3. Ross Singer's Solr Experiment

<a href="http://www.flickr.com/photos/ebyryan/473822132/" title="Photo Sharing"><img src="http://farm1.static.flickr.com/214/473822132_f92a5609ca.jpg" width="500" height="380" alt="Ross's Solr" /></a>

This Solr instance is interesting in the fact that it has more then just catalog data. While it has around 750k+ records in it, the records come from DSpace, the library catalog and EAD Finding Aids. He hopes to add Subject Guides and databases (e-resources). Dublin Core was used as a possible crosswalk and alignment of the disparate data. This leads to plenty of experimentation with ranking and display of information. It will be interesting to see something like this go live.

As for stats the development version was built by 1 person (Ross) mostly over a weekend. The instance runs on a 2GHz windows workstation. The interface is written in Ruby on Rails.

h3. Fac-Back-Opac

<a href="http://www.flickr.com/photos/ebyryan/473822084/" title="Photo Sharing"><img src="http://farm1.static.flickr.com/227/473822084_c24e23c7ab.jpg" width="500" height="379" alt="Fac-Bac-Opac" /></a>

This project is actually hosted on Google Code "so you can download it yourself":http://code.google.com/p/fac-back-opac/ if you want to play with the interface. It is written in python with Django. From the project page:

bq. The faceted backup OPAC project began with Casey Durfee's Open Source Endeca in 250 lines or less presentation at the code4lib 2007 conference, where he claimed to provide faceted features similar to the Endeca and AquaBrowser experiences using Solr and Django.

Again the project is running on modest hardware, a standard PC with 1.5GB of RAM which is also running DSpace. In my testing it was quite responsive.

h3. Project Blacklight

<a href="http://www.flickr.com/photos/ebyryan/473822078/" title="Photo Sharing"><img src="http://farm1.static.flickr.com/188/473822078_1598df0c4f.jpg" width="500" height="379" alt="Project Blacklight" /></a>

You can "read more about Project Blacklight at Bess' Blog":http://www.ibiblio.org/bess/?p=75 and here's a short description from it:

bq. We need significant data cleanup and rationalization to make the facets user friendly. But overall, I'm impressed with what we've been able to accomplish in a few months, with no offical committment of staff time, using only our spare time, borrowed hardware, and good will.

There is also a link to a demo at the blog. I suggest checking this out as it uses a similar interface to that of "NINES' Collex":http://nines.org/collex. What I'm talking about is the idea that everything is a facet, including your keyword. This means you start with the global facets already shown. You can add facets to limit things down, invert them to remove certain items and add keywords as additional facets. This makes it easier to do some more complex operations where you have some things excluded and some limited, without knowing the boolean or logic behind it. When you foray into the idea of using user-contributed or user-specific data, then it grows even more powerful. I could have the catalog show me things that were only in a certain location that matched my keyword that I hadn't checked out before or isn't on my current to-read list.

I still think it's a rather complex interface and can have a small learning curve to take advantage of all the features but it will be interesting to experiment with it to see how easy it can be made or how well people warm to the idea.

For the stats people there are 3.7 million records and..

bq. The marc records are indexing through a ruby script Erik wrote, directly from marc, without transforming into marc xml first. The box it's all running on is a development server, with four medium fast CPUs and 3.5G of RAM. Solr is running through Jetty, Blacklight is running on a pack of four mongrel instances, with apache doing load balancing out front. Sessions get written to a mysql database, and we use capistrano for deployment and versioning. And it sends us all an email every time an error gets generated.

h3. Rob Casson's Experiment

<a href="http://www.flickr.com/photos/ebyryan/473822128/" title="Photo Sharing"><img src="http://farm1.static.flickr.com/222/473822128_ac8c568147.jpg" width="500" height="380" alt="Rob's Solr Search" /></a>

Rob has also been playing with Solr and you can see the now familiar facets. He's also experimented with adding things like Refworks Export and item marking. One of the nice things about Solr is that it takes care of enough that it leaves time to experiment with the interface itself. Rob has also experimented with browse views using facets:

<a href="http://www.flickr.com/photos/ebyryan/473822126/" title="Photo Sharing"><img src="http://farm1.static.flickr.com/167/473822126_10f8829b8a.jpg" width="500" height="378" alt="Rob's Solr Browse" /></a>

It's an interesting use of facets and similar to that of Collex and Project Blacklight, though it gives different starting point interfaces for the different paths. Something to mess around with. For the stat people, this was a two-person job with Rob using the help of his Authority Control Librarian to help clean up the data and experiment. It's about 2 million records and mostly default install.

h3. Dave Pattern's Experiment

Dave is also messing around with Solr and was able to get something basic up in a couple hours of work. Be sure to "check out his blog":http://www.daveyp.com/blog/index.php/archives/202/ for info on his trials. I played with it briefly but haven't had a chance to do much with it. Link to a demo is there and I believe he plans on releasing the Perl source.

h3. Conclusion

Hopefully this gives you an idea of what people are playing around with and that it's not something you need a 20-person well-funded team to accomplish. Play around. There's plenty of people on #code4lib that are playing with Solr although I'm sad I haven't had the time yet to do more then interface experiments.
