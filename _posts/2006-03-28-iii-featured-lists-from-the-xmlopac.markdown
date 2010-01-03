--- 
wordpress_id: 211
layout: post
title: III Featured Lists from the XMLopac
wordpress_url: http://blog.ryaneby.com/archives/iii-featured-lists-from-the-xmlopac/
---
Featured lists are another thing I'd like to use more of. The ability to pull the latest books and other data from the server would be nice. While I figured out how to pull the information, the XML server appears to ignore my limiting and returns the whole list no matter what. This can be problematic if you have a large featured list. The way to get a featured list from the xmlopac is just take the list number and add a zero in front. <a href="http://magic.msu.edu/xmlopac/0337/1/1/1/5">Here's an example</a>. He's the same example <a href="http://ebyryan-2.user.msu.edu/dev/listmag/list.php?l=0337">in a slightly nicer display</a> (parsed). These links may break if the lists are removed. I figured out the list number by going to /ftlists in the opac, clicking on a list and then taking the numbers directly after the letters bib.

I'm hoping to make this a bit more useful with the item data but we'll see if I can figure out how to limit/paginate it first.
