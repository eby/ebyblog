--- 
wordpress_id: 462
layout: post
title: Item Display
wordpress_url: http://blog.ryaneby.com/archives/item-display/
---
There's a <a href="http://schoolof.info/infomancy/?p=340">nice post over at Infomancy about OPACs</a>:

<blockquote>The AADL SOPAC is, at its heart, an OPAC. And therein lies the problem. The purpose of an OPAC is to connect users with MARC records. Even if we connect them in a socially empowered environment, we are still connecting users with something that has no value to them. They are not looking for MARC records, they are trying to find resources. The back end OPAC that is powering the search for the SOPAC does not provide a positive finding experience.</blockquote>

AADL is still dependent on the III based OPAC which I think holds them back quite a bit. It will be interesting to see how they cope or move away from it. Some are playing with Solr and other technologies to make their own indexes, facets and interfaces. There's some trade-offs involved but the control may make up for it.

Another problem I tend to see with the "lipstick on a pig" type of path is that it is quite easy to go from some mild lipstick to something that looks like a dead hooker from a CSI episode. Though not as severe I've noticed this problem with Amazon and AADL as new pieces are added on. The new features are plugged into an old template and it becomes slightly harder to use. I believe AADL is currently working on a new item level template, I can only hope that Amazon tweaks things after they figure out the plog/wiki/tags/etc then are doing. Here's an example result from AADL (click for larger image):

<a href='http://blog.ryaneby.com/wp-content/uploads/2007/02/aadlresults.png' title='AADL Results'><img src='http://blog.ryaneby.com/wp-content/uploads/2007/02/aadlresults.thumbnail.png' alt='AADL Results' /></a>

I found it rather disorienting as it's hard to see where I actually am. The title of the book gets kind of mixed in though the status is easy to spot. This was probably fine back when you were lucky to get that far in the OPAC but as deep linking becomes more possible it will become more important to be able to tell exactly where you are. This means more prominence to the title and other important information. You'll also likely need to make sure branding and other information is present.

David Walker, from a place warmer then Michigan right now, has been experimenting with a Solr index of his holdings which has allowed faceted search, etc with somewhat more ease than previous options. He's still scraping the MARC view for the item display but he's been able to pull off a simple interface, so far, with a little amazon data added. It will be interesting to see how it pans out once he adds more features.

<a href='http://blog.ryaneby.com/wp-content/uploads/2007/02/solrresult.png' title='Solr Result'><img src='http://blog.ryaneby.com/wp-content/uploads/2007/02/solrresult.thumbnail.png' alt='Solr Result' /></a>

Another project of his was Xerces which provides an article metasearch. Again the results are quite easy on the eyes.

<a href='http://blog.ryaneby.com/wp-content/uploads/2007/02/xerxesresult.png' title='Xerxes Result'><img src='http://blog.ryaneby.com/wp-content/uploads/2007/02/xerxesresult.thumbnail.png' alt='Xerxes Result' /></a>

Another nice piece in the screenshot above is the use of simple language like "we don't have it but...you can get it in x days" which is a lot more useful then some of the screens I see.

Both David and Blyberg are working on redesigns so I have no doubt that some great things will be seen in the future. They also are both working with open systems that will likely allow them to be more agile then they would otherwise. Once of the great things is that AADL can try out new stuff, keep it if it works or tweak it if need be without the time frames or problems that they would traditionally face.
