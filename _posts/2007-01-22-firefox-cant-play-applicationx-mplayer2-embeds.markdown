--- 
wordpress_id: 444
layout: post
title: Firefox can't play application/x-mplayer2 embeds
wordpress_url: http://blog.ryaneby.com/archives/firefox-cant-play-applicationx-mplayer2-embeds/
---
Had this problem with the home computer on Windows. Upgraded WMP but didn't help. The solution is to install two missing DLL files in the Firefox plugins directory. You'll likely need to restart Firefox. The DLL's were:

<ul>
<li><a href="http://www.dlldump.com/download-dll-files_new.php/dllfiles/N/npdsplay.dll/3.0.2.628/download.html">npdsplay.dll</a></li>
<li><a href="http://www.dlldump.com/download-dll-files_new.php/dllfiles/N/npwmsdrm.dll/9.00.00.3250/download.html">npwmsdrm.dll</a></li>
</ul>

Was a quick fix for me.

<ins>Update</ins>: Thanks to commenter's there looks like there's some <a href="http://kb.mozillazine.org/Windows_Media_Player">decent information available at the MozillaZine site</a>. They also <a href="http://www.microsoft.com/windows/windowsmedia/player/version64/plugin.aspx">link to an installer</a>, but that doesn't apparently work with Vista. If your still having problems check out the mozilla site.
