--- 
wordpress_id: 117
layout: post
title: Firefox Protocol Handlers
wordpress_url: http://blog.ryaneby.com/archives/firefox-protocol-handlers/
---
This is a tip I found back when I was having various problems with external applications not working with Firefox the way I wanted. It also helps if you want to create your own protocols for testing/development, etc.

By protocol what I mean is the URL prefix such as aim:// mailto:// etc. Usually when you install a program that uses it's own protocol prefix it will update your browser with the correct information. On linux and OSX though I've had mixed results and sometimes I want to send the information to other programs such as mplayer or VLC even on Windows. My original problem was with the Last.fm service whose radio player uses the lastfm:// protocol.

If you don't already know you can type about:config into the address bar in Firefox and get advanced settings. This allows you to highly tweak the browser if you wish. It also allows you to add custom settings which is what we need to do. The general layout is:

network.protocol-handler.external.protocol = boolean (true or false)
network.protocol-handler.app.protocol = /path/to/program

I've found that there is no need to do the external boolean in my testing just the app one. So to add the lastfm:// protocol you would go to about:config and then right-click somewhere and choose new > string. You would then enter the following information:

Preference Name: network.protocol-handler.app.lastfm
Value: /path/to/lasfm/player (/home/ebyryan/Downloads/lastfm/player in my case)

For windows it would likely be the "C:\dir\to\file" structure while OSX would have similar syntax to above (try terminal). You will likely need to restart firefox to notice the change. I've also used this to handle iTunes (itmss) protocols. If your in an internal setting where you control people's computers you could use this to create custom protocols for your intranet that launch specific software on the users computers when they click on items. Not sure how useful that is though.
