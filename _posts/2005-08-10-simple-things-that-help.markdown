--- 
wordpress_id: 39
layout: post
title: Simple things that help
wordpress_url: http://ebybox.aresgate.net/blog/?p=39
---
<p>I've been experimenting with <a href="http://wordnet.princeton.edu/">WordNet</a> (SQL version) and <a href="http://aspell.sourceforge.net/">Aspell</a> to see about adding spelling and synonym suggestions to the output from the III XML server. One of the things I love about google is the way it offers suggestions and allows you to easily fix your search. Many failed searches can be fixed this way and there has been times where I didn't know I misspelled a word until google told me. I really don't think there is a need to call the reference desk for help if it's just a simple mistake like that.</p>

<p>My trials are no where near showing right now but lo and behold <a href="http://dewey.library.nd.edu/morgan/">Eric Morgan</a> has created <a href="http://mylibrary.ockham.org/simple/">a simple SRU client</a> that uses the same things I am. His version searches a OAI repository instead but the features are applicable to any search. You can read his <a href="http://lists.webjunction.org/wjlists/xml4lib/2005-August/005532.html">overview of it in a XML4LIB posting.</a></p>

<p>What I really like about his implementation is his controlled dictionary. Instead of allowing the spell checker to always suggest things it only does it when the correct word is actually present in the data. It won't fix the spelling if there's no record that has the word in it. This would prevent two failed searches and not give the person the idea that the searched failed due to spelling alone. I do agree with his reasoning:</p>

<blockquote>What is really great about this technique is that the spell checker will only recommend words that are in the dictionary, and the dictionary is only built from words in your index. Consequently, every single suggested word should have at least one record associated with it.</blockquote>

<p>On the other hand I still like the idea of always fixing it. Yes it provokes another failed search but the person knows now that their query was misspelled and can be fairly certain that it is now correct. Also I would think it affects the thesaurus. If the person repeats the query with the correct spelling I think the thesaurus could then give alternates that might be useful. With an incorrectly spelled word I don't think the thesaurus would help.</p>

<p>My other caveat about it is that the alternate spellings and synonyms aren't clickable to do the search for those terms instead. This can be problematic with more complex queries so I'm not surprised but it would be something I'd love to see in a future version.</p>

<p>What I think this illustrates though is how little things can make a large difference in helping people find what they want. I think something as simple as this can go a long way in helping people recover from failed searches. I'm sure it will spawn another debate over dumbing down the interface and someone will yell that students should know how to spell if they are in college and know how to use a thesaurus and putting it in the OPAC is just letting them be stupid. I'll leave that debate for another day.</p>
<!-- technorati tags start --><p style="text-align:right;font-size:10px;">Technorati Tags: <a href="http://technorati.com/tag/customer service" rel="tag">customer service</a>, <a href="http://technorati.com/tag/library" rel="tag">library</a>, <a href="http://technorati.com/tag/opac" rel="tag">opac</a>, <a href="http://technorati.com/tag/SRU" rel="tag">SRU</a>, <a href="http://technorati.com/tag/services" rel="tag">services</a>, <a href="http://technorati.com/tag/xml" rel="tag">xml</a></p><!-- technorati tags end -->
