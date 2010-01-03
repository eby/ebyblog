--- 
wordpress_id: 209
layout: post
title: Podcasting and the LMS - Podcast2JS
wordpress_url: http://blog.ryaneby.com/archives/podcasting-and-the-lms-podcast2js/
---
Podcasting still seems to be taking off, especially in the academic worlds. I can say that I listen to podcasts quite a bit. While I still occasionally listen to audio at someone's site it's just convenient to have ones I like downloaded to my computer. I am one of the <a href="http://news.designtechnica.com/talkback109.html">supposed 80% that don't use a mobile device</a> for it. I do have an ipod but often prefer to listen to music when I'm wandering around. That doesn't mean I find it any less useful though, as it brings all the benefits of RSS to other forms of media.

As a former education major (and now distance learning support) I have a real interest in it's use in courses, especially ones online. Having this media in the form of podcasts/vodcasts/etc allows easy use by those that want the content. Students can subscribe to lectures (video or audio), articles or information (itunes supports PDFs) or just view the information in the course.

There was a talk on campus I think last fall regarding podcasts in our LMS (learning management system...blackboard, etc). Right now it is very difficult to include this sort of functionality right into the course and about all you can do is provide the link to the podcast or upload the files to the course yourself. This is far from ideal. RSS is in the same boat with our LMS as there isn't much support yet. You can bypass this by using some of the RSS2JS services that are out there. Unfortunately I couldn't find a similar services for podcasts, so I built a prototype instead.

In simple terms all it does it take a URL for an argument and then output the information via document.writes into the browser. This lets you include the information into any normal html page with no need of having server side parsing on the server in question. I also passed the enclosure URL to a flash-based mp3 player. In the screen below I'm using the Odeo flash player though there are many available out there and ideally you would have one customized for the institutions. I've blanked out the URL as it's not really production worthy. I'd be interested if someone created such a service though. Odeo currently offers HTML for individual shows but doesn't have anything for full feeds.

<a href="http://www.flickr.com/photos/ebyryan/118897246/" title="Photo Sharing"><img src="http://static.flickr.com/45/118897246_82cdc86f4d.jpg" width="500" height="349" alt="podcast2js prototype" /></a>

In the example above the feed only has one show but it allows you to specify how many and will have a seperate box for each. I also include a link to download the mp3 file in case someone wants to save a specific show. The point of this is to allow you to show the most recent shows right inside your course or site (opac, etc). I've also provided the information and links to allow the student or user to subscribe to the podcast in their aggregator of choice. This allows them to consume the audio how they see fit. If there is an enclosure that isn't an mp3 then I link to it instead as shown in the screen below.

<a href="http://www.flickr.com/photos/ebyryan/118897247/" title="Photo Sharing"><img src="http://static.flickr.com/41/118897247_8772a6df2c.jpg" width="500" height="176" alt="podcast2js prototype" /></a>

Something like this has many uses though I would really prefer something that is built in. I'd be interested if anyone has something production-worthy already done. Mine is more of a proof-of-concept hackjob, though it mostly works.
