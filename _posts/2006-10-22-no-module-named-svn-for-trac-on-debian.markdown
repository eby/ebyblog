--- 
wordpress_id: 394
layout: post
title: No Module Named SVN for Trac on Debian
wordpress_url: http://blog.ryaneby.com/archives/no-module-named-svn-for-trac-on-debian/
---
I recently updated by Debian testing box and it appeared to upgrade python to 2.4. Since then when I went to my Trac install and went to browser it gave an error that "no module named svn". With googling I found multiple places that went the route of manually installing svn and trac. Luckily I didn't have to go this route. All I had to do was:

<code>apt-get install libapache2-mod-python</code>

I run Apache 2 and this uninstalled the mod-python-2.3 and installed the new mod-python. Once I restarted apache all was well. Hope this helps someone. If it doesn't then I guess google cause I probably won't be of much help.
