--- 
wordpress_id: 494
layout: post
title: Retagging and Changing Logs in SVN
wordpress_url: http://blog.ryaneby.com/archives/retagging-and-changing-logs-in-svn/
---
Found a couple tips on <a href="http://jroller.com/page/TedHusted?entry=svntips01">Ted Husted's</a> blog. He recommends deleting the old tag and then doing another tag as trying to overwrite will do a merge. And so to have it for prosperity here is the command to change the log for a revision:

<code>$ svn propset --revprop -r 504523 
  svn:log "WW-1715 Branch for 2.0.x at Struts 2.0.6-SNAPSHOT r504196"</code>
