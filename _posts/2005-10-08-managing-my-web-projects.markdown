--- 
wordpress_id: 78
layout: post
title: Managing My Web Projects
wordpress_url: http://blog.ryaneby.com/archives/managing-my-web-projects/
---
Well I'm finally using version control for my web projects. As you may know I recently started using <a href="http://gregarius.net/">Gregarius</a>, and the SVN version thereof. <a href="http://subversion.tigris.org/">Subversion</a> was fairly easy for me to pick up and had some very useful features. Since I had subversion installed I went ahead and created my own repository for my projects.

I had planned to do similar quite awhile ago after reading a series of articles on managing web projects. I recommend giving them a read:

<ul>
<li><a href="http://allinthehead.com/retro/228/">The Joel Test for Web Development - Part 1</a></li>
<li><a href="http://allinthehead.com/retro/229/">The Joel Test for Web Development - Part 2</a></li>
<li><a href="http://allinthehead.com/retro/230/">The Joel Test for Web Development - Part 3</a></li>
<li><a href="http://allinthehead.com/retro/231/">The Joel Test for Web Development - Conclusion</a></li>
</ul>

Subversion itself is useful, but add-on <a href="http://projects.edgewall.com/trac/">Trac</a> and it's wonderful. At first I doubted whether this would even be worth it. Being a one man shop and doing internal projects made me think that just coding it would be enough. Version control was something for large, distributed projects. Using Trac at the Gregarius site and seeing <a href="http://decafbad.com/blog/2005/09/30/trac-rocks-like-a-really-rocking-thing">the review at 0xDecafbad</a> convinced me to give it a whirl. It did take a little bit to get used to but it's already coming in handy. Being able to run a simple command and seeing what I've changed is more helpful then I thought. I can now run my dev version and create patches for the live version with ease instead of overwriting it like I used to. If I happen to screw something up I can easily go back to whatever version I need.

Trac itself has a ticket system, wiki and nice tracking features (timeline, etc.). Again I thought this as overkill as how many bugs I find would be minimal, but the documentation gave the idea of using it to track everything about the project. I now use the ticket system to track what features I want along with bugs and the like. I assign the features to milestones/versions and assign a priority. It lets me easily see what features I want and how they are fairing. I can easily re-prioritize things and keep track of the big picture. I've only had it going for a few days but it's already working well for me.

I have my install behind authentication due to the projects being work/internal. To get an idea check out of <a href="http://svn.gregarius.net/trac/timeline">the Gregarius install</a>.
