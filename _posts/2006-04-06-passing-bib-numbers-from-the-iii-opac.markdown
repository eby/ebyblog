--- 
wordpress_id: 217
layout: post
title: Passing Bib Numbers from the III OPAC
wordpress_url: http://blog.ryaneby.com/archives/passing-bib-numbers-from-the-iii-opac/
---
For those III institutions not as adventurous as AADL, you may want to be able to pass the bib number for a record to your own scripts. In this way you can use the stock OPAC but still add functionality externally. I'll give an example below and some other ideas at the end.

So let's start with an example. Our library doesn't use the stock recall functionality. They prefer to do it themselves and so have a webform that patrons can fill out. But lets say we want to include a button or link in the OPAC that only shows up on specific criteria. This would likely be difficult in the stock set-up but if you use your own script coupled with the xml server you can pretty much set any criteria you want. You could have all items checked out and at least one requestable, only for books already checked out for a certain period of time, not available online, etc.

There are a couple ways to accomplish this, though in both you are passing the bib number to an external script. One is to wrape an image in a link with the image having the src of the script. The script then returns a button image if it matches criteria or a 1x1 blank pixel image if it doesn't, to prevent people from seeing or clicking on it. The other alternative is to have script tags where the src is your external script that document.write outs a link if it passes criteria or nothing if not, via javascript.

So how do you pass the bib number to an external script? The token for your template is &lt;!--{fieldspec:Fb081}--&gt; which I have to thank <a href="http://blyberg.net">John</a> for. There are a couple caveats with the token:

<ul>
<li>The token needs to be on it's own line</li>
<li>The token only returns the number and not the letter 'b'. This means your script needs to add the 'b' before searching the xml server</li>
</ul>

So an example link would be:

<code>
&lt;a href="http://myserver/?bib=
&lt;!--{fieldspec:Fb081}--&gt;
"&gt;Link to my script&lt;/a&gt;
</code>

So what are some possible applications you could build by passing the bib number and using the xml server? Well here's a few ideas:

<ul>
<li>Create maps of where things are located in the library</li>
<li>Create a wish-list application for patrons</li>
<li>A more robust export/citation manager</li>
<li>Create a stand-alone version of <a href="http://www.blyberg.net/2006/01/19/creating-a-virtual-card-catalog/">AADL's Virtual Card Catalog</a></li>
<li>Almost anything</li>
</ul>
