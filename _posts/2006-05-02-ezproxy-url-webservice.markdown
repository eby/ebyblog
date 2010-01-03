--- 
wordpress_id: 247
layout: post
title: EZProxy URL Webservice
wordpress_url: http://blog.ryaneby.com/archives/ezproxy-url-webservice/
---
A useful feature that was added to ezproxy is the addition to a xml based webservice which you can send a URL and it will return the ezproxy information if it's in the exproxy database or an false statement if not. This allows you to build applications that can go through URLs and rewrite them if they are valid resources. Think <a href="http://rsinger.library.gatech.edu/localizer/localizer.html">WAG the Dog Localizer</a>. We're currently migrating to ezproxy so this may come in handy with assisting people with updating links and verifying things are set-up properly. There's not much documentation on this feature but hopefully the following will help you. Thanks to Ross Singer for pointing out the feature and to Rob Casson for giving me the result schema.

<h4>To Enable It</h4>

Straight from the <a href="http://www.usefulutilities.com/support/changes.html">changelog</a>:

<blockquote>Adds ezproxy.cfg directive ProxyURLPassword to specify a password that activates new EZproxy's support to respond to XML request sent to /proxy_url.</blockquote>

<h4>Input Schema</h4>

From what I've seen this would be posted to the http://exproxyserver:port/proxy_url page. You can also use GET by doing /proxy_url?xml= followed by the request xml. If you use POST you will want to name your field as 'xml'.

<code>
&lt;?xml version="1.0"?&gt;
&lt;proxy_url_request password="secret"&gt;
&lt;urls&gt;
&lt;url&gt;http://www.somedb.com&lt;/url&gt;
&lt;url&gt;http://www.otherdb.com/search/&lt;/url&gt;
&lt;/urls&gt;
&lt;/proxy_url_request&gt;
</code>

<h4>Result Set</h4>

<code>
&lt;proxy_url_response&gt;
&lt;proxy_urls&gt;
&lt;url proxy=&quot;true&quot; scheme=&quot;http&quot; hostname=&quot;ezproxyserver&quot; port=&quot;2048&quot; login_path=&quot;/login?qurl=&quot; encode=&quot;true&quot;&gt;http://epnet.com&lt;/url&gt;
&lt;/proxy_urls&gt;
&lt;/proxy_url_response&gt;
</code>

Where epnet.com is the vendor name and the information regarding your ezproxy server is included as attributes. A response for a URL that should not be proxied would look like this:

<code>
&lt;?xml version=&quot;1.0&quot; encoding=&quot;UTF-8&quot;?&gt;
&lt;proxy_url_response&gt;
&lt;proxy_urls&gt;
&lt;url proxy=&quot;false&quot; scheme=&quot;&quot; hostname=&quot;&quot; port=&quot;&quot; login_path=&quot;&quot; encode=&quot;false&quot;&gt;http://www.google.com&lt;/url&gt;
&lt;/proxy_urls&gt;
&lt;/proxy_url_response&gt;
</code>
