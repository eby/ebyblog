--- 
wordpress_id: 412
layout: post
title: Future of the ILS Symposium
wordpress_url: http://blog.ryaneby.com/archives/future-of-the-ils-symposium/
---
I spent one of my days off this week at the <a href="http://infoservices.uwindsor.ca/ils/">Future of the Integrated Library System Symposium</a> in Windsor. As with most things <a href="http://librarycog.uwindsor.ca">Art</a> plans, it was worth the time. I'll probably be posting some more about some of the ideas that came about there but here's a brief run-down. 

<h4>Where we are</h4>

Thanks to detroit traffic and a hotel without parking, I missed the continental breakfast. There was plenty of coffee left thankfully. The even then started with a presentation by Art (<a href="http://infoservices.uwindsor.ca/ils/sessions/ils/">slides</a>). He used some analogies such as cars. Cars have become increasingly complex but have a support structure (diagnostics, etc) that have evolved with them. ILS's have gotten complex but have no such structure. He then went on to talk about the importance of evolution in library systems and not reinvention. He also decried the lack of metrics in many library areas. We know things are wrong but we don't really know much detail about what's really going on. Art's a big proponent of using specialized components and hooking them together. Many businesses are moving from monolithic to specialized software that talk to each other (more from pmurray later). Accounting has accounting software, not an accounting module hacked together for the sprinkler system. There is good software out there for acquisitions and workflows, why not use them and spend the effort on making great systems talk to each other. The general take-home message he had was that the backend needs work too, not just the opac.

<h4>SOA in Libraries</h4>

Following up on Art's ideas on the backend was Peter Murray's <a href="http://dltj.org/2006/11/windsor-soa-presentation/">talk on SOA in libraries</a>. I've read on SOA but haven't really kept up as I should. His main focus, that at least I picked up on, was the componentization of the ILS. Having discrete software that is specialized and have open protocols or paths for them to talk to each other. It fits well with the ideas Art has on using outside software and I also think such an architecture may be needed to allow rapid changes in workflow or collections, like the rise in ERM. There seems to be some work around NCIP and other ideas with some of the opensource ILS's that may help support such an architecture in libraries. I won't try to explain much else, browse <a href="http://dltj.org/">pmurray's blog</a> if you want more info. There may be better or alternative models, i'm not sure.

<h4>Evergreen and PINES</h4>

It was nice to finally see a presentation about Evergreen instead of just the blog and other reading. The talk revolved around the history of the project and the challenges they faced. It was interesting to see their requirements and what they did to resolve them. Solid engineering work. The system architecture was really nice to see and the amount of redundancy was more then I expected. The storage system does appear to be a weak point but that appears to be common these days with some businesses moving to Amazon S3. It was also impressive to see that they were able to overcome the political issues, such as global library policies, which I think likely kill many consortia ideas.

I think an important take-home is that they had very special needs and demands which most vendors aren't going to support just due to the business case. This is the prime area where home-grown and open-source solutions shine as the modifications or building can be done in house. Having an architecture that allowed them to do feature-requests in a day didn't hurt either. The reviews of the consortia project are good and I can only expect them to grow with the new software. Some links:

<ul>
<li><a href="http://gapines.org/">Evergreen catalog</a></li>
<li><a href="http://open-ils.org/">Evergreen development site</a></li>

<h4>Some other links</h4>

I then ducked out of the symposium to talk with Beth Jefferson of Bibliocommons. I'll save that for another post.

</ul><ul>
<li><a href="http://www.wallandbinkley.com/quaedam/?p=86">pbinkley's notes on the symposium</a></li>
<li><a href="http://www.pzed.ca/words/archives/2006/the-author-pines-for-georgia-pines/">Peter Zimmerman's notes</a></li>
<li>Blogwithoutalibrary has extensive notes on all the sessions: <a href="http://www.blogwithoutalibrary.net/?p=240">Art's intro</a>, <a href="http://www.blogwithoutalibrary.net/?p=242">pmurray's soa talk</a>, <a href="http://www.blogwithoutalibrary.net/?p=243">PINES/Evergreen</a>, <a href="http://www.blogwithoutalibrary.net/?p=244">Alan's talk on Scholarly Portals</a> (missed it myself), and <a href="http://www.blogwithoutalibrary.net/?p=245">the closing Q and A</a></li>
</ul>
