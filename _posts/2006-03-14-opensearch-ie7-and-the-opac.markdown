--- 
wordpress_id: 194
layout: post
title: OpenSearch, IE7 and the OPAC
wordpress_url: http://blog.ryaneby.com/archives/opensearch-ie7-and-the-opac/
---
You've probably seen <a href="http://www.daveyp.com/blog/index.php/archives/70/">Davey P's post about the IE7 auto-detection of OpenSearch</a>. Since I <a href="http://blog.ryaneby.com/archives/innovative-xml-server-opensearch/">already had a 1.0 instance for our OPAC</a> I went ahead and upgraded it to 1.1 and tried it out (IE7 doesn't seem to like 1.0). It's still just a simple xslt with the III XML server. The auto-detection worked as well as the searches I tried. Currently IÃ‚Â only haveÃ‚Â itÃ‚Â returningÃ‚Â RSSÃ‚Â thoughÃ‚Â itÃ‚Â couldÃ‚Â do ATOMÃ‚Â andÃ‚Â htmlÃ‚Â inÃ‚Â the future.Ã‚Â The obligatory screenshot:

<a href="http://www.flickr.com/photos/ebyryan/112519472/" title="Photo Sharing"><img src="http://static.flickr.com/38/112519472_70e7c0c885.jpg" width="500" height="375" alt="MAGIC in IE7 Beta" /></a>

My first impression was that it resembled the way Safari handles RSS feeds (which I like). I'm also warming to the idea that this is a good move. The toolbar searches are usually for simple keywords (google, amazon, etc) and using opensearch as the backend for that just makes sense. I'm hoping that more browsers will pick up on this idea so we no longer have to provide a Firefox search plugin, Opera search plugin, etc.

Another thing I like is that it makes it easy to subscribe to your search, though I could live with the information box being just a tad smaller. I haven't had a chance to play much with the IE7 beta but it is shaping up. The sites I work on still work so that's the biggest thing. Will have to play more in the future. If you have the beta you can <a href="http://libdev.ryaneby.com/opensearch11/">try out my test page here</a>.
