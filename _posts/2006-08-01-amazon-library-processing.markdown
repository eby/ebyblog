--- 
wordpress_id: 323
layout: post
title: Amazon Library Processing
wordpress_url: http://blog.ryaneby.com/archives/amazon-library-processing/
---
Amazon <a href="http://www.amazon.com/libraries">has launched their Librarian Store</a> They now offer approval ordering, corporate accounts for libraries and also "Library Processing".

<blockquote>Amazon is pleased to introduce Library Processing for Corporate Account customers. With this feature, you can receive mylar covers, MARC records, labels, and more with your Amazon.com orders. Reduce the time and effort it takes to get your books from the Amazon box to your library shelves.</blockquote>

What's interesting to me is that some of this is making it's way into the Amazon API. I checked today and there appears to be Subjects that look like LCSH and also Dewey information. Some examples for Agile Web Development with Rails: A Pragmatic Guide:

&lt;DeweyDecimalNumber&gt;005.117&lt;/DeweyDecimalNumber&gt;

&lt;Subjects&gt;
&lt;Subject&gt;Computer - Internet&lt;/Subject&gt;
&lt;Subject&gt;Computer Books: Web Programming&lt;/Subject&gt;
&lt;Subject&gt;Computers&lt;/Subject&gt;
&lt;Subject&gt;Internet - Web Site Design&lt;/Subject&gt;
&lt;Subject&gt;Object-oriented programming (Computer science)&lt;/Subject&gt;
&lt;Subject&gt;Ruby (Computer program language)&lt;/Subject&gt;
&lt;Subject&gt;Computer / Internet&lt;/Subject&gt;
&lt;Subject&gt;Computers / Internet / Web Site Design&lt;/Subject&gt;
&lt;Subject&gt;Computers / Programming / Software Development&lt;/Subject&gt;
&lt;Subject&gt;Web site development&lt;/Subject&gt;
&lt;Subject&gt;web, ruby, rails, ajax, framework client, server, development,lightweight scripting, better, faster&lt;/Subject&gt;
&lt;/Subjects&gt;

<ins>Update: Looks like I pasted over the via information. I got the pointer for the offering from a co-worker and the API pointer <a href="http://dilettantes.code4lib.org/2006/08/01/one-stop-shopping/">came from Ross</a>.</ins>
