--- 
wordpress_id: 251
layout: post
title: Protecting SVN Directories
wordpress_url: http://blog.ryaneby.com/archives/protecting-svn-directories/
---
I use SVN/Trac for quite a bit of my development including my web projects for work. Both the repository and trac is private as most of my projects are internal. For testing purposes I usually have a copy checked out to a public webserver of each project as it's a really easy way to prototype. One thing I didn't really think about was that the .svn directories are viewable if you don't take precautions. It mostly just has information like repository address and doesn't have things like the password but if your one that doesn't want any of that sort of information being public you can do some easy rules in Apache or elsewhere to deny access to these directories. There's a <a href="http://hivelogic.com/articles/2006/04/30/preventing_svn_exposure">nice article over at hivelogic explaining how to do this</a>.
