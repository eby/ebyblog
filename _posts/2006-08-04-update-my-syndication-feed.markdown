--- 
wordpress_id: 329
layout: post
title: "Update: My Syndication Feed"
wordpress_url: http://blog.ryaneby.com/archives/update-my-syndication-feed/
---
I went ahead and updated Wordpress to the newest version and decided to try to fix my feeds while I was at it. I've followed the syndication arguments since near the beginning though I've stayed out of it myself. Recently I've been working on parsing incoming feeds and have found out how terrible many are. <a href="http://www.librarywebchic.net/wordpress/2006/08/03/feeds-that-dont-render-properly/">Library Web Chic has also noticed some of these problems.</a> In order to try to do my part I've made some changes. I apologize for any aggregators marking things as new.

<h4>Only One Feed Format</h4>

One of the items that have come up in many discussions is for you to choose a format and support it. Offering the same content in multiple formats can just lead to confusion. It also leads to more work trying to keep things validated and working. You can still have more that one feed (comments, posts, etc) but should stick with a format. From <a href="http://blogs.msdn.com/rssteam/archive/2005/08/03/446904.aspx">Microsoft's best practices</a>:

<blockquote>Unless you have a really good reason, itÃ¢â‚¬â„¢s not a good idea to have two links (or three!) that provide the same feed in different formats. It just makes the user have to pick between two things that they are not capable of distinguishing between. Pick your favorite format, and just support that.</blockquote>

Nick Bradbury (of TopStyle and FeedDemon) <a href="http://nick.typepad.com/blog/2006/05/pick_a_format_a.html">also recommends this route for an additional reason</a>:

<blockquote>Even worse, I often see RSS and Atom feeds which contain the same content yet identify posts differently (i.e.: the GUID for a post in the RSS feed is different from the ID of the same post in the Atom feed). As a result, feed search engines show posts from both feeds as though they were different, which to end users looks like duplication.</blockquote>

All my feed URLs (outside of comments) should point to the same feed now.

<h4>Control over the Feed</h4>

Due to me changing domains and unstable hosting, I had moved my feed to feedburner. This gave me nice things like stats for subscriptions and items. Recently they changed their service, making the item URLs very ugly. This likely doesn't matter for many but my feed is announced in IRC. This, coupled with validation errors, has let me to stop redirecting to the feed. Right now I'm leaving the Feedburner feed up and working. However, I may remove it in the future. If you subscribe to that feed please change it to <a href="http://blog.ryaneby.com/feed/atom/">the new final one</a>. I will do my best never to move it again.

<h4>ATOM 1.0</h4>

During my work with syndication feeds I've found various problems that would cause anguish. The first thing I would do is to look and see whether it was valid to do something, so I would know whether I could complain to the creator or not, or if it was a bug in my code. I found the many RSS formats were fairly ambiguous. Usually it was much less so with the Atom spec. Due to this I have decided that the format I will support is Atom 1.0. I have modified Wordpress's feed to provide valid Atom, which supposed is slated for a future Wordpress release. My feed provides both excerpts and full text. If you use an aggregator such as Bloglines you should be able to display either. I'm uncertain about other aggregator support but Atom support seems to be getting better and better.

This, of course, was my choice based on my experience. You may choose to support something else. If you notice anything weird with my feed, please let me know in the comments. The comment feed is still RSS 2.0 and I'll likely change that in the future as well.

Remember to <a href="http://feedvalidator.org/">validate your feed</a>. Now I just need to do something about the website itself.
