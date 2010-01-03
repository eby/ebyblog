--- 
wordpress_id: 445
layout: post
title: "ILS Data: Evergreen"
wordpress_url: http://blog.ryaneby.com/archives/ils-data-evergreen/
---
A first post in hopefully a series. Access to data from the ILS has been a common thorn in #code4lib'ers sides. I'm hoping here to post some of the ILS's that are out there, what data access options they offer and whether they are built in the base or are extra products. I won't bother with costs or other sensitive info.

As the Evergreen crew is on #code4lib and don't appear to sleep, I'll start with them.

<h3><a href="http://open-ils.org/">Evergreen</a></h3>

<dl>
<dt>Export</dt>
<dd>Built in. Currently can dump MARC XML. Could do other crosswalks and they are being written as I write this.</dd>
<dt>Database Access</dt>
<dd>Built in. Database is standard PostgreSQL</dd>
<dt>API's and Web Services</dt>
<dd>Built in. Currently there are JSON and XML gateways, OpenSRF,  XMPP service, OpenSearch, XMLRPC and unAPI. These services are used by the product itself in various ways so should allow full access to data. Some of the formats that are supported include MODS, MARC XML, RSS, ATOM, oai_dc, srw_dc and rdf_dc. The format information was taken <a href="http://open-ils.org/blog/?p=51">from their blog</a>.</dd>
</dl>

