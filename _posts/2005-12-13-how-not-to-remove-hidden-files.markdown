--- 
wordpress_id: 141
layout: post
title: How Not to Remove Hidden Files
wordpress_url: http://blog.ryaneby.com/?p=141
---
Was cleaning up a harddrive I moved to a linux box and wanted to get rid of all the '.' files that OSX leaves around. An easy way to list the hidden files, or so it would seem, would be:

<code>find ./ -name ".*"</code>

And it would look correct. But unfortunately this also catches the filesystem pointer of "./" so if you pass it to, say rm -rf then you may recursively delete everything in that directory. In order to prevent this you need to specify "-type f" so that it doesn't catch the pointer. So:

<code>find ./ -type f -name ".*" -exec rm -f {} \;</code>

Should work a bit better. Of course, always have a backup.
<!-- technorati tags start --><p style="text-align:right;font-size:10px;">Technorati Tags: <a href="http://www.technorati.com/tag/backup" rel="tag">backup</a>, <a href="http://www.technorati.com/tag/linux" rel="tag">linux</a></p><!-- technorati tags end -->
