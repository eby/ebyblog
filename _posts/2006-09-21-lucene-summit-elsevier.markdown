--- 
wordpress_id: 364
layout: post
title: "Lucene Summit: Elsevier"
wordpress_url: http://blog.ryaneby.com/archives/lucene-summit-elsevier/
---
<a href="http://librarycog.uwindsor.ca:8087/artblog/librarycog/">Art</a> was kind enough to let me attend a Lucene Summit he was having in Windsor and since it was close I went ahead and attended. The summit started with some brief introductions of some of the problems <a href="http://knowledgeontario.ca/">Knowledge Ontario</a> (the organizer) is having with some of their digital search projects. Most were using <a href="http://lucene.apache.org/">Lucene</a> for their full text indexing and the talk revolved around related problems and products that seem to make things easier (<a href="http://flamenco.berkeley.edu/index.html">Flamenco</a>, <a href="http://incubator.apache.org/solr/">Solr</a>, etc.)

<h3>Elsevier, University of Toronto and Scopus</h3>

The first real session was hosted by some of Elsevier's skunkworks developers. It was really nice to see that a vendor like Elsevier has a developer group (although small) that gets into the quick prototyping and idea generation stuff. This presentation was on the adaption of Scopus to include local results. Here are some highlights:

<ul>
<li>Project focused on distributed search, mixed content types and adaption of the scopus UI</li>
<li>Looked at various search engines including <a href="http://www.marklogic.com/">Mark Logic</a> (xmldb) but settled on Lucene due to it's low overhead and other advantages. Since it was open-source they were able to modify quite a few things to work how they wanted</li>
<li>The distributed indexes included local index (done by the university) and the scopus index (done by elsevier). This allowed Elsevier to stay out of the local process and allow the university to take care of it. Even with servers in Toronto and Ohio, latency was low</li>
<li>They added extended boolean. The query parser would move outwards from any boolean word found to hopefully parse it better. The example given is a user typing "Boston Red Sox and Toronto Blue Jays" (without quotes) likely did not want their query to be Sox and Toronto.</li>
<li>They take care of any special operators that mean something to the engine, for example *,?,etc</li>
<li>They start by checking to see if it's a proper query with special operators, if not then they check for boolean and if it does appear to be structured properly then they move to parsing it as natural language</li>
<li>They added the ability to do pure NOT queries (everything that isn't something)</li>
<li>The default operator is AND</li>
<li>They added a proximity boost that boosts any documents with the words near each other. The examples gives appeared to be within the fuzzy 3 range (~3).</li>
<li>Example: Boston Red Sox --> (Boston AND Red AND Sox) OR (Boston Red)~3 OR (Red Sox)~3</li>
<li>They tokenized fields that could have multiple values, for example author names. This was to prevent something from coming up when they put in the first name of one author and the last name of another (example)</li>
<li>They stated they plan on releasing their Lucene changes as open source though there was no specific timeline</li>
</ul>

The presentation was interesting but probably the most to those who are working with distributed indexes as the project met quite a few problems included local vs global ranking and indexing differences.
