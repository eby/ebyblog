--- 
wordpress_id: 571
layout: post
title: Apache External Filters and PHP Sessions or Cookies
wordpress_url: http://blog.ryaneby.com/archives/apache-external-filters-and-php-sessions-or-cookies/
---
Not needed in most cases but an interesting tool for some special ones. You can take advantage of browsers sending cookies with HTTP requests under a domain by using External Filters in Apache to modify the content based on those cookies. For example below we filter the requests for a specific location through a PHP script that can read the $_SERVER['HTTP_COOKIE'], get the PHPSESSID, read the Drupal database or similar and modify the content depending on whether someone is logged in, anonymous, etc. 

<code>
<pre>
ExtFilterDefine myfilter mode=output cmd=/path/to/your/script.php
<Location /locationfoo>
    SetOutputFilter myfilter
</Location>
</pre>
</code>


The php script would contain the logic of pulling the data out of the cookie, connecting to the DB, modifying content, etc. There's better ways to do this most of the time but in certain circumstances it could be used for content filtering or faked single sign-on with proxying. Apache will pass the proxied page to the script in that case.
