--- 
wordpress_id: 231
layout: post
title: IE Crashes with Embedded Content
wordpress_url: http://blog.ryaneby.com/archives/ie-crashes-with-embedded-content/
---
We've gotten quite a few calls about this so I'll post here in case any one else notices the problem. We received multiple calls about Internet Explorer giving a dialog about allowing ActiveX and then promptly crashing once you hit OK. This happened with Quicktime content but it may occur with any content type.

After much research and deduction I narrowed it down to a windows update with ID of KB912812. This security update includes a non-security update with ID of KB912945. If you didn't know Microsoft lost a patent lawsuit with Eolas that led them to change how IE handled embedded content. In the process apparently they changed more then just adding a pop-up. After some more deduction I found that if you only have the EMBED tag without an OBJECT tag wrapping it IE will crash and burn. Add the OBJECT wrapper and everything is OK. I hope this helped anyone who is seeing this problem as well. There are also workarounds to get rid of the pop-up that uses Javascript but I was just happy to keep IE running. Here are some resources:

<ul>
<li><a href="http://support.microsoft.com/default.aspx/kb/912945">Internet Explorer ActiveX update</a></li>
<li><a href="http://www.microsoft.com/technet/security/advisory/912945.mspx">Microsoft Security Advisory (912945)</a></li>
<li><a href="http://www.microsoft.com/technet/security/Bulletin/MS06-013.mspx">Microsoft Security Bulletin MS06-013: Cumulative Security Update for Internet Explorer (912812)</a></li>
<li><a href="http://developer.apple.com/internet/ieembedprep.html">Apple: Preparing Websites with Quicktime Content for the IE Update</a></li>
</ul>
