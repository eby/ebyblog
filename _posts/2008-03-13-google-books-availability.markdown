--- 
wordpress_id: 584
layout: post
title: Google Books Availability
wordpress_url: http://blog.ryaneby.com/archives/google-books-availability/
---
As you've probably read elsewhere Google finally released <a href="http://booksearch.blogspot.com/2008/03/preview-books-anywhere-with-new-google.html">a way to get book availability on Google Books</a>. It's a fairly simple web service where you hand it an identifier and it gives back whether the book is on Google Books and how much so (no view, partial view, full view) along with cover images. AADL previously scraped for the information which I've now disabled and used the new API instead. It was fairly easy with a little jquery and small changes to catwrap. I'm not yet using ThingISBN/xISBN so the results aren't that great. LCCN/OCLC identifiers would probably also help.

And as <a href="http://www.librarything.com/blog/2008/03/google-books-in-librarything.php">Tim at LibraryThing</a> and <a href="http://bibwild.wordpress.com/2008/03/13/google-book-search-api/">jrochkind found</a> they seem to be going for basic and client side which limits what you can do with it. I haven't had time to look into what's allowed in terms of caching or how many requests per client before being shut down. It would probably help to do the calls server side and cache for all the lccn/oclc/isbn possibilities in the long run.
