--- 
wordpress_id: 441
layout: post
title: Upgrade to ATOM
wordpress_url: http://blog.ryaneby.com/archives/upgrade-to-atom/
---
As I recent posted there was a <a href="http://blog.netscape.com/2007/01/16/to-dtd-or-not-to-dtd/">debate over Netscape's decision</a> to remove the DTD's for older RSS types (0.9 and 0.91).

One of the outcomes of this decision is that the <a href="http://www.intertwingly.net/blog/2007/01/17/Use-of-RSS-DTDs-Deprecated">feed validator will now give a warning</a> if the DTD is linked to. The recommendation is to either upgrade to something else (RSS2.0, ATOM, etc) or remove the doctype and try validating again without it.

If you happen to be using one of those versions, now might be the time to upgrade to <a href="http://en.wikipedia.org/wiki/Atom_(standard)">ATOM</a>. Many tools already output it and you'll likely only need to change the templates to point to the ATOM feed instead of the RSS one. If you run Wordpress then <a href="http://benjamin.smedbergs.us/wordpress-atom-1.0/">there is a nice plugin</a> that will change all feed links to output ATOM 1.0. 

If your OPAC has RSS but you can't edit the templates, maybe now is the time to ask for the ability.
