--- 
wordpress_id: 92
layout: post
title: Library Service Security and Privacy
wordpress_url: http://blog.ryaneby.com/archives/library-service-security-and-privacy/
---
There was a <a href="http://www.technobiblio.com/archives/2005/10/spl_rss_feeds_security_snafu.php">recent post over at TechnoBiblio</a> regarding a <a href="http://www.seattlest.com/archives/2005/10/21/seattle_public_library_and_the_naked_feed.php">recent security problem</a> with the SPL RSS feeds. The patrons PIN and barcode were included in the feed (URL I believe). This was a mistake due to the fact that some people use web based aggregators that allow others to see their feeds. It's good to see that SPL recognized the problems and corrected it but it highlights a few areas that need to be considered when implementing services such as this.

One is user education. This is a new technology for many people and so they may not realize the consequences of making the data available. I use a few sites that have private feeds and they are covered in warnings about being careful about the feeds. With the increase in phishing and other problems I don't really think there is any technology where you can presume the user knows. What I've see done for feeds is that it is marked with a lengthy random key for a URL and the user can have the key/url regenerated if they believe it has been compromised. There is also a possibility of authentication though I'm uncertain of the support. Of course, non of this will prevent someone from using a third party site that may show their information so it is still best to have as little personal identity information in there as possible.

Another is privacy in general. You may be able to create great services by collecting as much data as you can and keeping the data but you need to be clear about what you are doing so patrons can make the choice. Some will want to have their data available as <a href="http://libraryelf.com/">LibraryElf</a> has shown but others would likely prefer to not have their history on file, especially with the recent library vs. feds/PATRIOT stuff going on. I believe it would be best to support both and have the data collection be an opt-in but right now I doubt few systems support conditional collection.

Libraries are obviously not the only ones making this mistake but it's important to pay attention to these issues. A privacy policy is nice but take the time to think about what data is needed and what isn't and where this data may end up.

If I sound critical it is because I've had three departments in our college notify me in the last year that my information was compromised. Most of these units had no reason to have that sort of information on file. My University seems to be getting a clue now about security but I'm sure there's plenty out there that haven't.
