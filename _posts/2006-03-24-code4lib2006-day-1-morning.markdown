--- 
wordpress_id: 206
layout: post
title: Code4Lib2006 - Day 1 - Morning
wordpress_url: http://blog.ryaneby.com/archives/code4lib2006-day-1-morning/
---
I should have posted this some time ago. There's supposed to be audio coming but I have yet to see it. This conference was full of information so I'm going to split up the posts. A <a href="http://www.code4lib.org/2006/schedule">schedule with links to presentations is available</a>.  If my memory is too vague feel free to comment and correct. I have to stress that this only gives you a small idea of the great information at this conference. The discussions at lunch and at the bar afterwards were just as informative and probably more so at time. I'll be posting more soon.

<h4>A virtual keynote by the Evergreen development team</h4>

<a href="http://open-ils.org/documentation/presentations/code4lib2006/code4libcon-pines-1.html">Slides (html)</a>

I was looking forward to this talk as I've followed the <a href="http://open-ils.org/blog/">open-ils blog</a> and think they are doing some interesting work, especially with the architecture (jabber, etc). The PINES consortia is a rather large state system. They found that the current vendor solutions did not meet their needs (wasn't designed for it) and began development of their own. They hope to release it so other libraries/consortia can use it as well. The system was designed from the ground up without much of the "library-centric" backgrounds one might expect. Catalogers and others were asked for their ideal workflow rather than implement the current workarounds they used with other vendors.

Another interesting note is that they are storing marcxml in the database but when they want to display it or index it they transform it to MODS. They only go to the original marcxml record when they need something that is not contained within the MODS version.  I believe they also stated they are using the PostgreSQL relevance ranking along with a few modifications.

<h4>ERP Options for Acquisitions by Art Rhyno</h4>

<a href="http://librarycog.uwindsor.ca:8087/artblog/librarycog/resources/erp/erp.html">Slides (html)</a>

I've followed <a href="http://librarycog.uwindsor.ca:8087/artblog/librarycog">Art's blog</a> for sometime as well and he's got quite a few interesting projects, including using Google Desktop to search library holdings. I can't say I understand much about the Acquisition side of libraries but the presentation still made sense. His main point seemed to be that ordering systems are very complex things with complex workflows and most ILS implementations are hacks or incomplete. Full-fledged ERP systems (non-library) would likely be a better investment and provide better workflows. Apparently quite a few libraries in Canada already do this.

<h4>unAPI talk by <a href="http://onebiglibrary.net/">Dan Chudnov</a></h4>

<a href="http://onebiglibrary.net/files/20060215-c4lc-unapi-opa.pdf">Slides (pdf)</a>

Since the conference this idea has taken off even more, but even then it was ramping up and I was interested in learning more. I haven't been keeping as good of track as I should and don't understand everything about it. My general understanding is that it is a simple microformat coupled with a simple API that allows you to move metadata for objects around. The <a href="http://unapi.info/">official site</a> says "unAPI is a tiny HTTP API for the few basic operations necessary to copy discrete, identified content from any kind of web application". Your best bet is to go through the examples on the site. The one thing that is clear is that there is a need for the ability to copy/paste information on the web similar to copy/paste on the desktop. There's also some <a href="http://weblog.infoworld.com/udell/2006/03/16.html">posts by Jon Udell</a> and <a href="http://lesscode.org/2005/10/21/baby-steps-to-synergistic-web-apps/">over at Lesscode</a> that may bring you up to speed on the issue.

<h4>WikiD talk by Jeff Young</h4>

<a href="http://www.code4lib.org/files/WikiDcode4lib.pdf">Slides (pdf)</a>

This was another talk I was really looking forward to. If you've seen OpenWorldCat then you've seen some of the potential for WikiD. WikiD takes the potential of wiki's and adds the potential of structured data. I also have written down that it incorporates ideas of OAI repositories as well. While this thing is way too advanced for anything I'd be playing with I got the definite impression that anyone working on digital library collections should be looking at this.

The whole data structure was interesting as well (if I understand it correctly). It can handle arbitrary xml schemas and it will store the data in that collection with that schema. For indexing it will use a uniform schema that you map your data to. There has also been a change apparently in SRU to allow updating. It seems like a nice example of using many of the standards that are out there (SRU/W, OpenURL, RSS, etc) and integrating them into a useful platform.

I've probably just fed you with a bunch of misinformation so your best bet is to look through the slides, check out <a href="http://www.oclc.org/research/projects/wikid/default.htm">the project site</a> and an <a href="http://alcme.oclc.org/wikid/FrontPage">example site</a> (use firefox).
