--- 
wordpress_id: 493
layout: post
title: Trac Performance
wordpress_url: http://blog.ryaneby.com/archives/trac-performance/
---
In the past I've used mod_python to serve trac and got ok performance, but my installs weren't public. On Code4Lib it was set-up as a fcgi install. This worked ok but was extremely resource intensive.

I also host through TextDrive and found that they <a href="http://manuals.textdrive.com/read/book/8">recommend running Trac through Tracd and then proxying the requests through apache</a> if you want it on the normal port. I went ahead and tried that on code4lib. Trac seems responsive and the system didn't go to a crawl while it was being accessed. We'll see how it does in the long run.

If you run trac you might want to give it a try.
