--- 
wordpress_id: 582
layout: post
title: Twitter at AADL
wordpress_url: http://blog.ryaneby.com/archives/twitter-at-aadl/
---
I've been on and off <a href="http://twitter.com">twitter</a> quite a few times. It never really caught on with me. I commute between two different cities and most of my contacts are elsewhere in the world. The majority of the ones I meet up with aren't on the site nor are technology inclined. I do see the usefulness of the service for time and location aware information, though. A few things I wish for:

<ul>
<li>MDOT feed of lane/road closures on my commute route</li>
<li>Alerts from my favorite bars when happy hour, new tap, etc happens</li>
</ul>

There's actually already a commuter aggregator called <a href="http://www.commuterfeed.com/">CommuterFeed</a> which looks interesting and I remember reading at least one story about a DOT using twitter. <a href="http://twitter.com/flyingdog">Flying Dog</a> is on twitter but i see quite a few business possibilities. Slow hour at the pub? Twitter a special on beers for the next 20 minutes (presuming you have foot traffic).

Quite a few libraries also got on twitter. David Lee King has at least <a href="http://www.davidleeking.com/2007/05/09/twittering-libraries/">a partial list</a>. Most have gone the route of using rss2twitter or similar to send out additions to their sites, etc. I didn't really see the major benefit of that so I've stayed away from it. I do see the benefit of doing some announcements on it, especially since the audience may be the kind that want's to try out beta quality apps or are technology friendly.

The big use I see are for events. Since we've recently rehauled our event backend I thought I'd try hooking it into Twitter. Since there is a <a href="http://www.aadl.org/node/9928">PHP class</a> available for the api, it became really quick and easy to try things out. Now 30 minutes before each event a tweet is sent out as a reminder. I've also sent out a few manual tweets asking for feedback on some quick iCal feeds and alerts of some videos added to the site (also built on the new events system). You can follow at <a href="http://twitter.com/aadl">twitter.com/aadl</a> if you think you would get benefit from it. The route will likely be towards a SMS/IM bot type of application.

Here are some of the other ideas I've had, some more feasible than others. <a href="http://vielmetti.typepad.com/superpatron/">Ed</a> has also been helpful with trying things out and giving some feedback.

<ul>
<li>Notices of event cancellations / library closures</li>
<li>Direct Messages of when holds are ready for pickup</li>
<li>Direct message to put a hold such as "d aadl hold 1580538908"</li>
<li>Message for hours, etc</li>
</ul>

There's quite a few possibilities for mobile/time/location dependent services a library provides that show potential. You'll probably see quite a few posts about the event system in the future. It has become the backbone of quite a few services including our recently launched <a href="http://www.aadl.org/video">streaming video</a>. Once iCal is done I'll probably move on to hcal Atom service or similar for building external apps on.
