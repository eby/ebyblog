--- 
wordpress_id: 337
layout: post
title: Search Data and Feed Security
wordpress_url: http://blog.ryaneby.com/archives/search-data-and-feed-security/
---
Two things that are worth looking at and thinking about.

First is <a href="http://www.techcrunch.com/2006/08/06/aol-proudly-releases-massive-amounts-of-user-search-data/">news that AOL released a data set of users' searches on purpose</a>. The data was partially anonymized but since some of the searches can be identifying in themselves it's possible that this might turn into a privacy fiasco for them. There also seems to be reports that there's sensitive data such as social security in it. If you do search analysis or other data mining, think long and hard how to anonymize and protect data.

The second is about using feeds as vulnerability vectors. I believe this was presented at blackhat but <a href="http://www.spidynamics.com/assets/documents/HackingFeeds.pdf">a PDF with information is available</a>. This is nothing ground breaking as most aggregators use browser engines to display the information, similar to some email clients. Aggregator clients that run locally on a machine may also be considered to be in a less restricted zone. Something to think about if your building aggregators or parsing feed. As always you can't trust everything that's given to you. And as always be careful about what you subscribe to, as you would with email.
