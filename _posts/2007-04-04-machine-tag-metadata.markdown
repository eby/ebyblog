--- 
wordpress_id: 502
layout: post
title: Machine Tag Metadata
wordpress_url: http://blog.ryaneby.com/archives/machine-tag-metadata/
---
Once referred to as "tripletags" supposedly but now called Machine Tags, due to Flickr's adoption of their use for geocoding, etc. From <a href="http://machinetags.org/wiki/Main_Page">machinetags.org</a>:

<blockquote>Machine tags, or triple tags, are tags that are made up of three parts (namespace:predicate=value) in order to give extra information. Machine tags have been in use for a while now on sites such as Flickr and Upcoming.org to make information (such as location and event information) accessible to both machines and humans.</blockquote>

While still using the tag name, it's slightly more controlled and has some interesting potential. While their main use seems to have been the geocoding your probably familiar with, others are beginning to expand it's use to pull information from various API's into their software or sites. <a href="http://www.clagnut.com/blog/1907/">From clagnut</a>:

<blockquote>About a year ago I wrote about how tagging had become more than just a way to annotate content with keywords. Tags had become the wires by which disparate content could be connected. Through use of consistent and detailed tagging, I could begin associating my blog posts with my content on other web sites, such as my Flickr photos and my ma.gnolia links.</blockquote>

But what you'll probably find more interesting is the discussion of book tagging:

<blockquote>This time last year I was tagging photos and posts which discussed books in the following manner isbn=0713998393. In and of itself this works fine, but it is not a valid machine tag, which means we cannot make use of the afore-mentioned API goodness within Flickr (and where Flickr is leading so others will follow). We therefore need a triple-tag version of the ISBN tag, and here's my suggestion: iso:isbn=0713998393. ISBN is a standard recognised by the International Organisation for Standardization (ISO) so I thought it made a certain sense for ISO to be the namespace. Other standardised entities could be tagged in a similar way, such as iso:issn=15340295.</blockquote>

<a href="http://adactio.com/journal/1274">Adactio has a nice follow-up article on the use of machine tags</a> with flickr and blog posts, including the benefit of having custom namespaces:

<blockquote>I'm not restricting the search to just my photos, either. Any photos tagged with adactio:post=[ID] will show up on http://adactio.com/journal/[ID]. In a way, I'm enabling comments on all my posts. But instead of text comments, anyone now has the ability to add photos that they think are related to a blog post of mine......I realise that I'm opening myself up for a whole new kind of spam. But any kind of spam that requires namespaced tagging on a third-party site is pretty dedicated.</blockquote>

There's <a href="http://geobloggers.com/archives/2007/01/24/offtopic-ish-flickr-ramps-up-triple-tag-support/">also a nice post over at geobloggers about some of the possibilities</a>. And if your an RDF fan there's the <a href="http://weblog.scifihifi.com/2005/08/05/meta-tags-the-poor-mans-rdf">poor man's RDF</a> post you may find worth reading.

<h2>Libraries</h2>

Those is libraries are probably familiar with namespaces and <a href="http://info-uri.info/">info uri's</a>. Maybe they'll be submitted as a namespace on machinetags.org, who knows. Another <a href="http://efoundations.typepad.com/efoundations/2006/10/dctagged.html">similar use is that of "dctagging" by Pete Johnston</a> (thanks to edsu for the link):

<blockquote>So based on the Geotagging approach, I switched to using a convention I've informally called "dctagging" where I apply a tag dctagged and then use structured tags of the form dc:xyz=sssss, where each such tag represents (using the terminology of the DCMI Abstract Model) a statement using a property from the Dublin Core metadata vocabularies, with the property URI represented by the "qualified name" dc:xyz (actually, I use names of the form dcterms:xyz as well) and the value string is represented by the sssss part of the tag. So for items created by Tim Berners-Lee, I use the tag combination

dctagged dc:creator=Berners-LeeTim</blockquote>

Presuming the API's are decent, I can see quite a bit of potential for pulling together data from disparate sources for augmenting records and other data. A library's flickr photos of an author's visit can be easily shown on record pages in the catalog.  A work with geo-location data could not only be mapped but also have photos and events from modern day. While there are other ways to accomplish the same thing, machine tags have the potential to make it somewhat easier and use a larger community. I think it would be interesting to see what data could be added to the view of <a href="http://orlabs.oclc.org/Identities/">WorldCat Identities</a> if dublin core machine tags started being used. Photos, online texts, etc.

Just some thoughts, I haven't gotten around to playing with them yet. And if you didn't notice <a href="http://maps.google.com/maps?q=http://slashgeo.org/index.rss">Google Maps now supports GeoRSS sources</a>.
