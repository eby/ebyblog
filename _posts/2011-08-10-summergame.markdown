--- 
layout: post
title: Under the Hood of the AADL Summer Game
categories: code4lib
date: 2011-08-10 18:00:00
---

Cross-posted from the [AADL Devblog](http://www.aadl.org/node/41356) and written by our lead developer [ejk](http://twitter.com/ejk)

The 2011 Summer Game has brought big changes to the way we play here at the library. In addition to the "classic" summer reading game, players can earn points for writing reviews, adding comments and finding game codes at events and locations. Players also earn badges for special accomplishments. We just passed player ID #4000 and we still have weeks to go for even more players to join and earn points and prizes. The pieces that make up the Summer Game are diverse but by adding custom code to the solid foundations provided by these open tools we've been able to concentrate our efforts on adding new content and functionality rather than chasing bugs and putting out fires. Here's some of the tools and technologies that make up the Summer Game:

[Drupal](http://drupal.org/): The aadl.org websites run on the Drupal Content Management System. In addition to giving us a framework for writing blogs, creating user accounts and writing comments, it has a extensive API which allows us to leverage those pieces to add our own functionality. A drupal module for Summer Game was created that keeps track of player data, lets players add points through multiple activities, and displays a leaderboard. Players are attached to user accounts, and a simple function which could be placed in any code that runs the site allows us to award points for any website action. The summer game module is available through github: [Summer Game module](https://github.com/aadl/Summer-Game).

[Ubercart](http://www.ubercart.org/): The Summer Game shop runs on this Drupal module that provides a simple shop interface for your Drupal site. Again, it has a extensive API which allowed us to use Summer Game points as a custom payment type. We also added a hook into the order process to send data to our custom label printing function, printing labels for the items at the time of order, and creating custom order emails. By leveraging the ubercart module, we were able to create a complete online shop and order fulfillment process in about 3 weeks, start to finish.

[FPDF](http://www.fpdf.org/)/[FPDI](http://www.setasign.de/products/pdf-php-solutions/fpdi/): The core of the Summer Game is still the "classic" summer reading game, where you read books, fill out a score card, bring it to a library location and get a prize. This year we decided to track all our score cards with unique identifier numbers to see where and when people picked them up. We also wanted to allow players to print their score cards on demand as PDF files. The FPDF library allows us to dynamically create each score card PDF with a unique number. We also use the FPDF library to create easily-printable Game Code signs so staff can post a points-accruing Game Code at their events. The FPDI plugin for FPDF allows you to import an existing PDF as a template for your FPDF document.

[Redis](http://redis.io/): Redis provides a persistent data store, similar to a database, but as key-value pairs rather than tables. We used Redis to store the score card identification numbers because it allowed us to do an atomic increment operation. We don't want two people printing score cards at the same time with the same ID number. In a single call we can get the next number in the sequence without worrying about holding other people up or both grabbing the same number. We also use Redis to store our shop email notification data in a processing queue which allows us to delay sending them out. We currently use the [Redisent PHP library](https://github.com/jdp/redisent) to talk to our Redis install.

[Twilio](http://www.twilio.com/): Twilio provides an easy API to interact with users via cell phone text messages. By creating a simple drupal module that utilizes the Twilio API we allowed players at an event to easily sign up for the game and start earning points using their cell phones. We also use twilio to send prize pickup reminder text messages when we fill orders from the Summer Game shop.

AADL is happy to share source code. View the rest of our shared code on our [github page](https://github.com/aadl). Code monkeys not included. Your mileage may vary.
