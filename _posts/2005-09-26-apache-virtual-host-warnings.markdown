--- 
wordpress_id: 70
layout: post
title: Apache Virtual Host Warnings
wordpress_url: http://ebybox.aresgate.net/blog/archives/apache-virtual-host-warnings/
---
For awhile now Apache2 has been giving me the following warnings:

<pre>NameVirtualHost *:80 has no VirtualHosts</pre>

I finally got off my ass and figured out that the problem was that each of my virtual host files had the <pre>NameVirtualHost *:80</pre> on the top of it. I had created one virtual host and had used it as a template for the others. I moved the declaration to the actual apache config before it loads the virtual host configs and that got rid of the error. Wanted to post in case others are getting the warning and wondering what is causing it. Having modular configs are nice but forces you to be careful about the declarations. There's probably some config cleaning I could do as well.
