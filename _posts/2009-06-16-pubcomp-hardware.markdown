--- 
wordpress_id: 595
layout: post
title: Public Computing with Windows Servers and Linux Thin Clients - Hardware
wordpress_url: http://blog.ryaneby.com/?p=595
---
(also posted on the <a href="http://www.aadl.org/devblog">AADL devblog</a>)

<a href="http://www.flickr.com/photos/ejk/2636115429/"><img src="http://farm4.static.flickr.com/3279/2636115429_d15372d71a.jpg" alt="Computers at Traverwood Branch" /></a>

We recently overhauled the public computing setup at <a href="http://www.aadl.org">AADL</a>, though it hasn't been rolled out at all the branches yet. It consists of a mix of linux hosted web management software, linux thin clients and windows terminal servers. It is a bit of a unique setup so figure I should share. Once we get it farther towards complete we'll probably release the code. 

<h4>Some History</h4>

For some background the previous setup consisted of windows thinclients and windows servers running Citrix. The thin clients had published application sets that connected to a fairly basic server farm. The farm wasn't really setup well resulting in high loads and slow logins. A custom set of flash applications and php gateways administered it all.

As I researched options I decided I wanted to drop Citrix as I didn't really see it as needed and the licensing costs aren't exactly small. I also decided I would prefer as much be opensource as possible though we decided on keeping Windows for the public facing part for now.

I tested out quite a few public computing management software, lockdown software, cyber cafe software but didn't really find anything that did everything I wanted, kept it fairly simple, was flexible, etc. For reference here are a few things about our setup:
<ul>
	<li>Patrons can use the computer as long as they want without interruption unless there are other patrons waiting for a computer. They have a minimum 30 minutes if there is a line, after which they are given 5, 2, 1 minute warnings.</li>
	<li>They can be idle for a total of 10 minutes before being ended (given a warning after 5)</li>
	<li>They swipe their card at an assigner first that gives them a station. These are spaced out then random</li>
</ul>

<h4>The New Thin Clients</h4>

<a href="http://www.flickr.com/photos/ejk/2616603311/"><img src="http://farm4.static.flickr.com/3199/2616603311_018ba08858.jpg" alt="Debian Thin Clients" /></a>

The thin clients we settled on are <a href="http://h10010.www1.hp.com/wwpc/us/en/sm/WF05a/12454-12454-321959-338927-89307-3634729.html">HP Compaq t5735 Thin Clients</a>. In bulk they ran under $250 each. The specs worked out for what we needed:


* VESA mountable on both sides. Made it easy to securely mount to tables and even to the back of monitors
* 1 GB Flash, 256M RAM
* VGA and DVI
* Lots of USB ports including back, front and secure (within case)
* Debian Linux preinstalled (stock plus some custom HP packages)


The thing I like most about the thin clients is the imaging process. The clients come with a HP programs called HPThinState which can write a bootable imager to a USB drive. Once the USB is imaged you can boot other machines from the USB and walk through a simple imaging process. The process is simple enough that front line staff now image machines themselves when needed (usually ext3 partition corruption after power failure). This has significantly cut time of IT staff and reduced how long a client is out of order for simple problems.

Another nice thing is that all changes are put on flash immediately, no special write/flashing software needed. You can apt-get upgrade and have the changes there on reboot with no further interaction.

<h4>Break Out Boxes</h4>

One of the biggest problems we had previously was USB ports being damaged on clients. We tried multiple things like hubs, etc but nothing really lasted. Our latest attempt is using a modular box that is meant to be inserted in a 5.25 cd bay on a tower. We put 2 usb extenders and a headphone jack extender in it and mount it to the table. This leaves an easily replaceable port and also lets us move the thin client out of harms way. So far this has worked great and we haven't had to replace a port yet. At about $10-12 it can't be beat.

<a href="http://www.flickr.com/photos/ejk/3463165138/"><img src="http://farm4.static.flickr.com/3633/3463165138_cf779e2cb5.jpg" alt="Modular USB Boxes" /></a>

<h4>Other Hardware</h4>

We have USB floppy drives available for use and may expand to other formats. The monitors are stock though we add on privacy screens. Each station is also equipped with a USB based barcode reader that is used for signin purposes.

We also have one of the thin clients VESA mounted to a monitor and barcode reader that acts as the assigner.

More information on the actual software / workflow behind it coming up in a second post. Overall though we've been really happy with the hardware described above. Really stable and much better priced.
