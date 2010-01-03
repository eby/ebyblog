--- 
wordpress_id: 65
layout: post
title: "Reminder: Back up Your Data"
wordpress_url: http://ebybox.aresgate.net/blog/archives/reminder-back-up-your-data/
---
Awhile ago I had some data lose on some library servers. I had presumed that the data had been backed up by those running the server. No more. I've been slowly implementing backup procedures for the various servers my department has data on. Still got a lot of work to do.

Well two days ago another server crashed (hdd failure) and, big surprise, the supposed backups failed. Luckily I had a copy of our stuff to put back up. The other departments...probably not as lucky. I house my backups on my server (this one) and thought to myself, damn I better make sure everything is backed up onto a third computer. I also better make sure that the blog and sites and everything are currently backed up.

Well long story short I went to backup this site and bam, hard drive failure. At least I thought so as there were DMA timeout errors. It ended up being a bad cable from the power supply. Switched cables and ebybox is back in business. What amazes me is that ebybox is around 7 or 8 years old (400Mhz P2) and still running on the original hardware, including harddrives. This was a computer I put together myself so it has a bit better hardware than some.

My friends? Not so lucky as they have mostly newer harddrives which seem to drop like flies every few months. It used to be that there were certain brands you could trust but now adays it seems your gambling when you choose a drive and if your lucky it'll last. I'm afraid to upgrade the drives in my server as I just don't trust any of the current ones out there (unless you drop some big moolah for enterprise level drives). I'm all for increasing capacity but at least make it so I can trust putting shit on the thing. My friend had 3 large drives in a RAID and they all went at once. Kind of hard to recover data from that.

Well the lesson here is back shit up. Not only that but do it to different computers. I may be looking at <a href="http://www.strongspace.com/">Strongspace</a> here in the future once we start putting more critical operations online. I apologize for the downtime. There may be more in the future if I end up having to replace the power supply.

Update: A <a href="http://www.mezzoblue.com/archives/2005/09/22/web_server_b/index.php">timely article at Mezzoblue</a>. I was setting up rsync at the time this came across.
