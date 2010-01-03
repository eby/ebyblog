--- 
wordpress_id: 95
layout: post
title: The Utility of Library Blogs
wordpress_url: http://blog.ryaneby.com/?p=95
---
A <a href="http://www.tametheweb.com/ttwblog/archives/001850.html">recent post at Tame the Web</a> caught my eye. The <a href="http://www.libraryjournal.com/article/CA6269278.html">article he links to</a> has quite a few good recommendations. I'll address one of the quotes on TtW first:

<blockquote>Despite the rapid proliferation of library blogs I was skeptical about their value and doubted that college students were ready for them. Nevertheless, in fall 2004 I began experimenting with a blog for the Paul J. Gutman Library at Philadelphia University. My skepticism, it turned out, was warranted. In an informal survey, I found that fewer than five percent of the respondents had even heard of RSS (real simple syndication) or news aggregators.</blockquote>

Alone, this statement is rather misleading but was used great in the article to push the use of RSS elsewhere. RSS does not need a blog and blogs don't have to have RSS. Blogs make it easier to create RSS feeds and allow the ability of having a dedicated site. However, if you want to just create RSS feeds so that people can pull in content to the library homepage, courseware, etc there are desktop tools you can use to create the RSS files. It's often simpler to just use a free blog service though some people may find it easier to use a desktop product or prefer not to have a separate site. Some example software (I haven't used so no recommendations):

<ul>
<li><a href="http://www.reinventedsoftware.com/feeder/index.html">Feeder</a></li>
<li><a href="http://www.phelios.net/rss-writer.html">RSS Writer</a></li>
<li><a href="http://www.usablelabs.com/productFeedSpring.html">FeedSpring</a></li>
<li><a href="http://www.feedforall.com/">FeedForAll</a></li>
</ul>

Also tying the value of the blog with the value of the feed is also a bit pushing it. There are plenty of people who actually visit a blog to read it and not subscribe to the feed. I read too many sites to actually visit them. Also the survey results aren't surprising in light of other surveys out there. For example these two:

<ul>
<li><a href="http://www.clickz.com/stats/sectors/search_tools/article.php/3555441">More Use RSS Than Have Heard Of It</a></li>
<li><a href="http://blogs.zdnet.com/ITFacts/?p=8996">83% are not aware they are using RSS</a></li>
</ul>

Despite this, RSS has the ability to really bring information to people even if they aren't aware of it. Having the ability to put timely, relevant information into courses, portals, anywhere is a boon. And this can be anything including events, announcements, etc. Our university uses RSS for their system status alerts so that the information can be syndicated on sites that need to let their users know. Mail server going down for emergency maintenance? A single update puts the information everywhere it needs to be. I currently pull the alerts in to our intranet and a portal instance as we handle the calls when there's a problem.

The article recommends the use of RSS2JS services and I have to agree. I've used it on various sites (portal) due to the fact that server-side parsing was not available. I still prefer to do the parsing myself with <a href="http://magpierss.sourceforge.net/">MagpieRSS</a> so I don't depend on external services or javascript support but that's not always possible. The code is available for many of the JS converters so you if you can find a server to host it on then you can rest easier. Here are a few of the services out there:

<ul>
<li><a href="http://jade.mcli.dist.maricopa.edu/feed/">Feed2JS</a></li>
<li><a href="http://itde.vccs.edu/rss2js/build.php">Feed2Js (same code - different host)</a></li>
</ul>

If you go to the <a href="http://jade.mcli.dist.maricopa.edu/feed/index.php?s=more">more section of the first Feed2JS</a> there is a list of alternate services though many are ad supported. A google search for rss2js or feed2js may find more.

I've written a similar parser for podcasts and have been experimenting with pulling those into courses. If I get anything that's not alpha quality I'll try to post it.

I guess that the take away message, as it is in the article, is to not write-off the blog just because only a few people visit it. Use it wisely and <em>USE THOSE FEEDS</em> and you might be adding value even if you don't know it. There are some tips for blogging at the bottom of the article. I recommend reading the whole thing.
