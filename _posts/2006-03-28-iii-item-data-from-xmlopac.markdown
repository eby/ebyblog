--- 
wordpress_id: 210
layout: post
title: III Item Data from XMLopac
wordpress_url: http://blog.ryaneby.com/archives/iii-item-data-from-xmlopac/
---
Before I forget to post this, David Walker was nice enough to drop me info on how to get the item information when getting bib results from the XML server. You can do this by appending the option of links=i1-10 to the end of the url. You also need to make sure you do the noexclude for the III data as the item records are part of it. I'm not sure if i1-10 limits the number of items but that's my guess. <a href="http://magic.msu.edu/xmlopac/.b3629461a/0/0/1/5?avsrank=D&noexclude=WXROOT.Heading.Title.IIIRECORD&links=i1-10">Here's an example.</a>

It returns some interesting and potentially useful information such as number of checkouts, renews, etc for that item. You can see an <a href="http://libdev.ryaneby.com/iiirecord/index.php?bibnum=b3629461a">example of some parsed output here</a>. If you need more bibnums to try just <a href="http://magic.msu.edu">search magic</a> and it will be listed in the perm link url.

I think David Walker is likely working on some interesting things with this. I have many ideas on how to use this information. This also takes us one step closer to replicating many of the opac features in our own software or metasearch applications.
