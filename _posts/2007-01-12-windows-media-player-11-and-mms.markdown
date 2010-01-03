--- 
wordpress_id: 434
layout: post
title: Windows Media Player 11 and MMS
wordpress_url: http://blog.ryaneby.com/archives/windows-media-player-11-and-mms/
---
A new semester and some new problems. The first is Windows Media Player 11. Not yet out via Windows Update so not a huge problem but with the coming release of Vista I think it will be.

I think it was reported in a few places but WMP11 seems to have removed support for the MMS protocol. You can see <a href="http://www.microsoft.com/windows/windowsmedia/licensing/netprokit.aspx">a chart showing this on their network protocol kit page</a>. It says that it can be used as a <a href="http://msdn2.microsoft.com/en-gb/library/aa390673.aspx">rollover protocol</a> but that doesn't appear to work, at least not in my testing though it may be a server configuration issue. 

In my testing I had to change the URL in the ASX file to specify RTSP as well as remove any port statements. The file then worked in WMP11 thanks to Helix serving it on that protocol as well.

A rather abrupt change as most streaming servers appear to use it for windows media files. We got kind of lucky here as Helix will stream the file over rtsp or http without too much problem. The hurdle is changing the ASX file generation it does on the server to include the proper link.

If you have streaming windows media files you may want to check and make sure they play on the latest WMP. 
