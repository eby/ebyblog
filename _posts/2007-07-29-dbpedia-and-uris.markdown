--- 
wordpress_id: 546
layout: post
title: DBpedia and URIs
wordpress_url: http://blog.ryaneby.com/archives/dbpedia-and-uris/
---
Found quite a few new things today via <a href="http://planetrdf.com/">Planet RDF</a> which included <a href="http://ivanherman.wordpress.com/2007/07/29/from-wikipedia-uri-s-to-dbpedia-uri%e2%80%a6/">a post about using URI's to identify music items</a>:

<blockquote>The question I had: what URI should I use for J.S. Bach's Well-Tempered Clavier? This is a non-trivial question if one wants to use, say, the Music Ontology in cataloging one's music: indeed there is nothing like, say, ISBN-s in classical music. I am not sure who suggested in the past that using the corresponding Wikipedia URI might be the best option we have. Well, now that we have DBpedia, I thought that the corresponding DBpedia URI (the non-informational resource one, that is) should be a much better choice. But what is the URI?</blockquote>

The <a href="http://musicontology.com/">Music Ontology Specification</a> is available online and licensed under a creative commons license and it looks quite interesting in what it is trying to accomplish:

<blockquote>The Music Ontology is an attempt to link all the information about musical Artists, Albums and Tracks together: from MusicBrainz to MySpace. The goal is to express all relations between musical information to help people finding anything about music and musicians. It is based around the use of machine readable information provided by any web site or web service on the Web.</blockquote>

Also pointed to from the post is <a href="">DBpedia</a>:

<blockquote>DBpedia.org is a community effort to extract structured information from Wikipedia and to make this information available on the Web. DBpedia allows you to ask sophisticated queries against Wikipedia and to link other datasets on the Web to Wikipedia data.</blockquote>

If your building catalogs with Wikipedia data integrated into it you may look at using DBpedia. The SPARQL examples make it look promising with queries like <a href="http://wikipedia.aksw.org/index.php?qid=1">Soccer player with tricot nr. 11, playing for a club having a stadium with >40.000 seats, born in a country with >10M inhabitants</a>.

Back to the post, the discussion is centered around the problem with having URI alias' for a single item like Wikipedia does. What is authoritative URI that should be used for identification. DBpedia does not have aliases which makes it clear though translating URI's from Wikipedia to DBpedia can be a more involved process because of it.

Regardless, it's interesting to see the things that are going on in the semantic web area and how all the data can be linked together and it's potential for discovery and catalog displays.
