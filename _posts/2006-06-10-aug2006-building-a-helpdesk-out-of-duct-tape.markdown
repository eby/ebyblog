--- 
wordpress_id: 278
layout: post
title: "AUG2006: Building a Helpdesk out of Duct Tape"
wordpress_url: http://blog.ryaneby.com/archives/aug2006-building-a-helpdesk-out-of-duct-tape/
---
This presentation was about having a helpdesk on absolutely no budget (on the side). In this case it was for the Southwest Virginia Education and Training Network which includes quite a few different schools and grade levels. They wanted a timely helpdesk but due to the finances could not do 24/7. There are really only two main people doing support. At first it was by a department email. They then created a problem tracker within ANGEL as a nugget on their My Page.

<ul>
<li>Person submits form. Has quite a few required fields such as course, instructor, etc. Some of this is used to validate identity for password problems</li>
<li>If within ANGEL it fills in some information</li>
<li>Ticket is opened in database and staff is emailed</li>
<li>Staff replies within ANGEL. User emailed as well as staff. Problem closed</li>
<li>Searchable, statistics, etc</li>
<li>Database is new tables within ANGEL's</li>
</ul>

I've been working on a similar design for our helpdesk though not integrated in ANGEL. I'd prefer to pull in information into the staff interface using some sort of API along with our other SIS systems. Would be good to have the submission form within ANGEL insert more useful information automatically for troubleshooting.
