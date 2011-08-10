--- 
layout: post
title: Summer Game Prize Fulfillment Workflow
categories: code4lib
date: 2011-08-10 19:00:00
---

Cross-posted from the [AADL Devblog](http://www.aadl.org/node/41426)

The [AADL Summer Game](http://play.aadl.org) has an online shop where earned points can be spent on awesome schwag. To try to make it easy for the volunteers and staff to fulfill the orders we took advantage of some of the infrastructure we already had in place for other parts of the site.

As some know our hold notices currently go through a script that sends an email along with printing a custom label to a label printer, that is used for identification on our hold shelves. We reused this process to print a custom pickup/order label everytime an order comes through the [ubercart](http://www.ubercart.org/) game shop by hooking into the payment process. This leaves a spool of order labels that those doing fulfillment can pick up throughout the week and start filling. A spool that has been increasing dramatically in length recently.

<a href="http://twitpic.com/5lqj65" title="The Summer Game Shop is live and we have our first order labe... on Twitpic"><img src="http://twitpic.com/show/thumb/5lqj65.jpg" width="150" height="150" alt="The Summer Game Shop is live and we have our first order labe... on Twitpic"></a>

As orders are filled the barcode on the custom label is scanned, which sets the order as fulfilled and adds a notification job to a [redis](http://redis.io) queue. Players have the option of getting SMS notifications (sent through [Twilio](http://twilio.com)) or email. Shop keepers can also cancel orders if need be which refunds the points to the player account.

After the items are delivered to the branch destinations on Friday morning, a script goes through the jobs on the redis queue and sends the notifications letting players know their items are ready for pickup.

<a href="http://twitpic.com/5mozzd" title="Our first batch of Summer Game stuff  (380,000 points worth),... on Twitpic"><img src="http://twitpic.com/show/thumb/5mozzd.jpg" width="150" height="150" alt="Our first batch of Summer Game stuff  (380,000 points worth),... on Twitpic"></a>

More background info on our [Summer Game](http://play.aadl.org) is in the works and keep that order spool growing!
