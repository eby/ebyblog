--- 
wordpress_id: 276
layout: post
title: "AUG2006: Extreme Action and Triggers"
wordpress_url: http://blog.ryaneby.com/archives/aug2006-extreme-action-and-triggers/
---
This presentation was by Victoria Neeshan of Independence University which is completely online, rolling enrollment. They've used the ANGEL actions to automate many processes and to allow large courses to be taught by a single professor. Students are given constant feedback during the course and the professors are emailed updates when needed. One example given was the final exam which is proctored.

<ul>
<li>First the student fills out a survey stating they are ready to take the final and asks for their assigned proctor email</li><li>
</li><li>On submit it emails the coordinator, sets an environmental variable for student with the proctors email and another variable for the exam as ungraded.</li>
<li>The coordinator then grades it as 100 which sets a random password using a formula to the environmental variable for the exam, emails the student that they can meet with their proctor and take the exam and also emails the proctor (using the previous variable) with the random password. The password includes a '!' which hides the exam until ready.</li>
<li>The proctor inserts the password into another quiz which explains other details which then unlocks and unhides the exam</li>
</ul>

Prior to using ANGEL and actions this process was much more convoluted and it often took a week before students heard back. Now it is hours or a day. I really don't think we use actions to the full benefit and will definitely have to play more with them.
