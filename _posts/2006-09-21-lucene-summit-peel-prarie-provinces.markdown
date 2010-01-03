--- 
wordpress_id: 365
layout: post
title: "Lucene Summit: Peel Prarie Provinces"
wordpress_url: http://blog.ryaneby.com/archives/lucene-summit-peel-prarie-provinces/
---
The next presentation at the Lucene Summit was regarding the trials and tribulations of the <a href="http://peel.library.ualberta.ca/">Peel's Prarie Provinces</a> project. Here are some notes:

<ul>
<li>Started with OCLC's SiteSearch</li>
<li>Outsourced digitization to OCLC and Olive, which gives xml based information with pixel positions of words in the images</li>
<li>Nice timeline view when doing a search (facet)</li>
<li>xml -> cocoon -> xsl -> display - allows multiple display formats including MARC output that other libraries can use to include the data (way to give back to those who help)</li>
<li>For newspapers: xml -> cocoon -> svg -> batik -> jpeg/png (<a href="http://sourceforge.net/projects/martini">martini project</a>)</li>
<li>These workflows give some flexibility and i18n abilities but have some scalability and scope problems, especially the svg portion</li>
<li>They index both forms of words that have special characters (with and without diacritics).</li>
<li>Store in an intermediate format to make it easier to index?? Appeared to be more compressed then the native Olive data</li>
<li>Differences in newspapers versus monographs can cause difficulties. Newspapers tended to have poor metadata/images (no article data)</li>
<li>Grouped pages under work. So search that has hits on multiple pages of a work would bring up one hit with multiple pages instead of multiple hits</li>
<li>Some of the facets could be done by pulling info as results came in but this created a large performance hit</li>
<li>Moved to Solr with cocoon - data mining, internationalization, better facet performance and helped with dynamic metadata</li>
</ul>
