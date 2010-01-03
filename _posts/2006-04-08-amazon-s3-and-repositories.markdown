--- 
wordpress_id: 221
layout: post
title: Amazon S3 and Repositories
wordpress_url: http://blog.ryaneby.com/archives/amazon-s3-and-repositories/
---
I have to admit that I ignored <a href="http://aws.amazon.com/s3">S3</a> when I first heard about it. Simple storage? I was certain there would be applications like backup utilities and companies using it to host data in cases where transfer was just too expensive with the local ISP or similar. Nothing I'd likely ever use, though.

However I should have known better, especially with how much I've used Opensearch. Opensearch simplified the reuse of results, expanded syndication and gave new ideas for interfaces. It's likely that S3 will do similar for online storage and repositories. There were a couple of things that changed my way of thinking.

The first was a <a href="http://aws.typepad.com/aws/2006/04/using_s3_to_sto.html">post on the AWS blog</a> regarding the addressability of objects in S3. The thing that really caught my eye was that you could retrieve the metadata for an object without requesting the object with a simple http request. This fits in with the idea of using it as an object repository.

The second is that there are already <a href="http://code.whytheluckystiff.net/parkplace/wiki">people building clones of the interface</a> for local storage. This opens up the possibility of hosting your own storage while using the many tools that are already being built to use the interface. It also gives me the impression that this may become a defacto standard for online storage and repositories similar to how opensearch is becoming a defacto standard (probably more so with IE7).

I have to admit that I still don't fully have my head around all of the ideas. I see potential for things like LOCKSS, dig libs, etc.

Some further reading:

<ul>
<li><a href="http://aws.amazon.com/s3">S3</a></li>
<li><a href="http://aws.typepad.com/aws/2006/03/firefox_s3_some.html"></a>Firefox + S3: Some Ideas for Developers</li>
<li><a href="http://aws.typepad.com/aws/2006/04/more_s3_crunchy.html">More S3 wrappers</a></li>
<li><a href="http://www.holovaty.com/blog/archive/2006/04/07/0927">How I'm using Amazon S3 to serve media files</a></li>
<li><a href="http://www.talkcrunch.com/2006/03/24/episode-3-amazons-new-grid-storage-service/">Talk Crunch Podcast on S3</a></li>
<li><a href="http://www.postneo.com/2006/03/22/backing-up-flickr-photos-with-amazon-s3">Backing Up Flickr Photos with Amazon S3</a></li>
<li><a href="http://weblog.infoworld.com/udell/2006/03/22.html#a1411">Towards politically neutral infrastructure: Amazon's S3</a></li>
<li><a href="http://www.magpiebrain.com/archives/2006/03/21/amazon_s3">Is Amazon S3 the first Tier 0 Internet Service?</a></li>
<li><a href="http://del.icio.us/tag/s3">del.icio.us / tag / s3</a></li>
</ul>
