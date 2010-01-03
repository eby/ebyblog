--- 
wordpress_id: 196
layout: post
title: III OPAC Hold Request URLs
wordpress_url: http://blog.ryaneby.com/archives/iii-opac-hold-request-urls/
---
A terrifying title I'm sure. Unfortunately I'm not graced with <a href="http://open-ils.org/blog/?p=51">SuperCat</a> with such things like a bookbag api so I have to work with III url's which aren't pretty. I've recently been requesting quite a few books through our union catalog and wondered if there was a way to easily link to the request pages. My ideal would be to set-up something similar to a netflix queue where I could easily request the next book on my list. I can link to the record pages and then click to request it but a couple less clicks would be nice.

For various other reasons that probably won't be possible with the union catalog without more work but in the process I figured out what appears to be a reusable URL structure for requests based on bib/record numbers. These URLs will take you to the request page where you enter your information or pick a location, etc. Someone else may be able to figure out how to enter your information, though be careful about how you pass PIN/passwords if required.

So here's a sample URL:

http://youropac/search/.b1341013//1,1,1,B/request~b1341013

For some reason you have to repeat the bib number 2 times. I've tried simpler combinations of the above and haven't been able to simplify it much without breaking it. You can also include characters between the // which is what III does but it appears to work without it. You do need the extra slash though to prevent a 404. Here's an example with all 3 bibs:

http://youropac/search/.b1341013/b1341013/1,1,1,B/request~b1341013

From what I can tell this does a search for the bib and then goes to the request. I can't seem to get it to work by going straight to the bibrecord with record=.

Regardless this comes in handy if your using the III XMLOpac and want to generate links for requests. Here's an <a href="http://libdev.ryaneby.com/request/request.php?q=genetics">example using Cal State's XML Opac</a>. Casey has also <a href="http://www.plymouth.edu/library/opac/record/1341013">added links in his WPOpac</a> (in link list on right hand side of a record). Another problem is it doesn't seem to always load the opac template when you follow the link, at least in my browser. It does when you refresh though.

If anyone knows a better URL structure feel free to comment. Oh and iii--
