--- 
wordpress_id: 274
layout: post
title: "AUG2006: Don't Play It Again Sam"
wordpress_url: http://blog.ryaneby.com/archives/aug2006-dont-play-it-again-sam/
---
This presentation was by Peter Friesen of Plattsburgh State University of New York and probably had the most take-home ideas of any. The presentation went over problems and workflows that were just too complex to expect faculty to complete.

Originally a <a href="http://sln.suny.edu/index.html">SLN</a> (apparently lotus notes based??) user they moved to ANGEL and experienced some problems getting the data moved over. His solution was to transform content to an ANGEL Archive that could then be imported by the professor. He used XSLT among other things.

A second problem was Word HTML that many tried to copy and paste into the LMS which usually caused formatting problems. His solution was to use regex to strip some of the problematic tags and again transform it into something professors could easily upload.

A third problem was multimedia. While most can do recording, to give a good experience for an online course they prefer to have it encoded in multiple bitrates and uploaded to a streaming server. They also like to include synced transcripts,SMIL,etc. His solution was to create a program using the Window Media SDK that would convert the media file for the professor. The application then takes their credentials and uploads the file to the streaming server, which automatically creates a playlist file. The application then takes this information and creates a HTML page with the embedded information and any metadata information the instructor included and posts it to ANGEL as a normal ANGEL Lessons Object (the professor can choose where to publish it to). We also have a streaming server so I found this very interesting as a help with workflow. He accomplished this by creating an ASP page that acts as an API for him, posting information to the database and returning some of the lists as XML.

Seeing some of the workflows that are possible with some small hacking (there is an actual API that might be usable instead) gives me hope that quite a few problem/advanced areas we have could become alot simpler in the future. Desktop integration would be one. I had also played around with the ANGEL Archive format and had played with some XSLT for it but I can see now that it may be even more useful that I thought and worth messing around with.
