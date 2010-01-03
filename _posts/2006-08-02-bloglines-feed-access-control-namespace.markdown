--- 
wordpress_id: 326
layout: post
title: Bloglines Feed Access Control Namespace
wordpress_url: http://blog.ryaneby.com/archives/bloglines-feed-access-control-namespace/
---
<a href="http://www.bloglines.com/about/specs/fac-1.0">Bloglines has released a namespace for specifying access control for your feed</a>, presuming you provide RSS 2.0 or ATOM.

<blockquote>To 'allow' access means a feed may be redistributed to other public sources, including search. To 'deny' access means a feed should not be redistributed to other public sources, including search. The default relationship is to allow access. However, if a feed is currently set to 'deny', the relationship must be explicitly set back to 'allow' for it to be registered (Simply ommiting it from the feed is not sufficient to turn access back on).</blockquote>

This also presumes the software you use allows customization of feeds. Not sure if this will catch on with other aggregators.

Libraries should still be careful about what content goes into feeds, but this offers a mechanism to help prevent accidental sharing of even non-identifiable data.
