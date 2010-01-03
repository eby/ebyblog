--- 
wordpress_id: 224
layout: post
title: Library Camp - Encouraging Patron Hacking
wordpress_url: http://blog.ryaneby.com/archives/library-camp-encouraging-patron-hacking/
---
For more information on Library Camp <a href="http://wiki.library2.net/index.php/Main_Page">check out the Library2.0 wiki</a>.

This discussion went over the various hacks and problems that allow patrons to reuse information from the library or make it easier to use the library's offerings. Some notes:

<ul>
<li><a href="http://weblog.infoworld.com/udell/stories/2002/12/11/librarylookup.html">Jon Udell's LibraryLookup Bookmarklet</a> helps people move between Amazon and the OPAC. Problems included that it's dependent on the site and can break. It's also dependent on ISBN. There are <a href="http://weblog.infoworld.com/udell/2006/01/30.html#a1378">Greasemonkey scripts that use xISBN</a> to try to get around this limitation. Also requires user installation which can be more demanding</li>
<li><a href="http://www.bookburro.org/">Book Burro</a>, a Firefox extension, allows checking a few large libraries as well as comparing prices. Has similar limitations as above. Also is not as easily modified for your library as a greasemonkey script.</li>
<li>Including the OPAC search in the browser search area. Opera and Firefox are fairly easy. I've written up an <a href="http://libdev.plymouth.edu/post/31">example of how to do it with OpenWorldCat</a> for Firefox. IE7 will support OpenSearch as a method <a href="http://blog.ryaneby.com/archives/opensearch-ie7-and-the-opac/">which I've posted an example before</a> using the IE7 beta. This has the benefit of being easy to install and also allowing people to subscribe to results.</li>
<li>Getting data out of the OPAC to play with. The simplist would be modifying templates to have microformats for scraping. More advanced options include <a href="http://www.blyberg.net/2006/01/26/major-enhancements-for-patron-rest/">AADL's REST interface</a>, OpenSearch, RSS/ATOM, SRU, etc. Lots of potential services, some of which overlap. Things like the III XML server help make these services possible.</li>
<li>There were some brief mentions of COinS and unAPI though it's a bit confusing to many. I don't think OpenURL was mentioned at all. I think it was related to buzz more than anything.</li>
<li>Potential problems with all of the services would be universal item id. Pre-ISBN data as well as other media types lack ID's that can be used at all sites. IMDB and Amazon may have different ID's for the same movie. IMDB may be becoming the adhoc standard. I believe one library is already beginning to code this information into the MARC record. I think it was <a href="http://cadl.org">CADL</a> but I'm not certain.</li>
<li>Patron annotation could become more and more useful. Use of other API's could also help make services more personal</li>
</ul>

The take away message was that libraries need to be where the patrons want them to be. This could be links in IMDB and Amazon or RSS feeds that can be used to set-up SMS alerts. Data needs to be simple and reusable.
