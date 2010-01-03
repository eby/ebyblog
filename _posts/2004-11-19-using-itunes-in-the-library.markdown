--- 
wordpress_id: 3
layout: post
title: Using iTunes in the Library
wordpress_url: http://ebybox.aresgate.net/blog/archives/using-itunes-in-the-library/
---
<img src="/blog/images/itunes.jpg" alt="itunes and your library" class="center" />

I recently came across <a href="http://www.tametheweb.com/ttwblog/archives/000520.html">a post on Tame the Web</a> that discussed the possibility of using iTunes at a library to serve audio files to patrons. The benefits can be numerous, but some limitations have to be kept in mind. I'll first discuss the possibilities of such a venture, then the quirks.

<!--more-->

The benefits for small libraries are probably minimal. The possibilities are the most promising for institutions that have a large audio archive and the ability to digitize the audio if need be. Any library can allow patrons to listen to music, but if the library has a audio archive it becomes a way of advertising the holdings of the institution.

An example of this would be the <a href="http://vvl.lib.msu.edu/">Vincent Voice Library</a> at Michigan State University. This archives consists of thousands of audio items. If a server was provided for that department to feature certain recordings, it may bring users that would have never thought of using the service. An example would be speeches by Civil Rights activists during Black History Month, speeches by Einstein during the recent anniversary of his work, and other special events. Music is also a definite option, especially during appreciation months, etc. An additional benefit is the seamless experience for patrons. All they have to do is plug into the network and load iTunes. They may even discover the resource on accident.

There are various things that have to be kept in mine if something like this was implemented. Firstly iTunes itself only allows 5 computers to connect to it with sharing (last time I checked). This is due to the limitations on sharing iTunes store material, but applies to sharing in general. A possible way around this might be to use a compliant server such as <a href="http://www.deleet.de/projekte/daap/daapd/">daapd</a>. I'm not sure if the server has similar limitations as iTunes.

This limitation brings up the possible problem of copyright. While the music is streamed to the client and not downloaded and is limited to the subnet of the server, I could see this as being construed as a public performance. Being a library and being used as an educational reason, it might fall under fair use, but this is definitely something that would have to be looked into before implementing a system. Public domain material is always an option and this could be the perfect way to expose patrons to older, more obscure material they might not hear otherwise. 

A few other problems exist. The protocol used to broadcast is limited to the same subnet as it will not make it past routers without some additional tinkering. More information on that can be found on the <a href="http://www.deleet.de/projekte/daap/daapd/">daapd</a> site. Another problem is the use of iTunes on public PC's. In small libraries this may not pose a problem, but in larger institutions it may become a problem as users try to load their own mp3's or similar onto the system, or not realize why it's there. An alternative to that is <a href="http://www.cdavies.org/applerecords.html">AppleRecords</a>, a open-source client that connects to the daapd server and allows the streaming of the material (and that's about it). Patrons with their own laptops with iTunes can just access it with what they have. Bandwidth is also an issue depending on usage.

As a quick wrap-up, the possibilities are interesting, but if such a project was undertaken, it would be important to plan it out as it is not as simple as loading songs onto iTunes and hitting share, unfortunately.
