--- 
wordpress_id: 291
layout: post
title: Data Fidelity and Bit Rot
wordpress_url: http://blog.ryaneby.com/archives/data-fidelity-and-bit-rot/
---
Think about the various software you use, including the ILS. Can you get your data out? Probably. But can you get it out without using that specific software or a vendor supplied solution? Could you write a script that converts the raw data on the system to another format? The answer is probably too often no.

I've personally lost email over the years due to outlook deciding it didn't like the old files. 3rd party scripts did little better. I've also lost various other data due to corruption or migration. My real concerns for this problem only came when I started working with library related things such as the ILS, Citrix, etc. The closed nature of everything and the multitude of walled silos of information was rather depressing. Wasn't this supposed to be a place of information exchange and preservation? Apparently only in carbon form.

Mark Pilgrim, of <a href="http://diveintomark.org/">Dive into Mark</a>, is finally back blogging and I recommend reading the following posts and try to remember these points:

<blockquote>Fidelity is not a binary thing. Data can gradually degrade with each conversion until youÃ¢â‚¬â„¢re left with crap. People think this only affects the analog world, like copying cassette tapes for several generations. But I think digital preservation is actually much harder, in part because people donÃ¢â‚¬â„¢t even realize that it has the same issues.</blockquote>

<blockquote>Data readable by only one application is a big risk factor, because the application wonÃ¢â‚¬â„¢t be around forever. If that application only runs on one operating system, thatÃ¢â‚¬â„¢s even worse, because the operating system wonÃ¢â‚¬â„¢t be around forever either. If that operating system only runs on one hardware platform, thatÃ¢â‚¬â„¢s even worse still. No hardware lasts forever, and you may eventually need to resort to emulating the hardware in software. Emulation is the ultimate fallback. But if any or all of those layers are closed, emulation may be costly or even impossible. And if any of the layers are DRM-encumbered, emulating them may be illegal. </blockquote>

<ul>
<li><a href="http://diveintomark.org/archives/2004/05/14/freedom-0">Freedom 0</a></li>
<li><a href="http://diveintomark.org/archives/2006/06/02/when-the-bough-breaks">When the Bough Breaks</a></li>
<li><a href="http://diveintomark.org/archives/2006/06/16/juggling-oranges">Juggling Oranges</a></li>
</ul>

Another important idea in all this is that open-source doesn't necessarily mean open-format. It's less of a hurdle but documentation is a requirement. I've found this especially true with the III xml server. You can get quite a bit of data out, presuming you know how. I've found it similarly frustrating tracking down quality documentation for some of the various library formats. Some of the specs are less than straightforward.

And then there are the cases where the implementations aren't to spec or the vagueness of the spec causes problems across data stores. If I gave you MARC data from many institutions you'd probably spend some time taking care of differences among them. There's also the case of vendors extending things without documentation or going their own way. I recommend giving Sam Ruby's <a href="http://www.intertwingly.net/blog/2006/06/18/Accidentally-Closed">Accidently Closed</a> post a read.

<blockquote>Openness is not a binary quantity.  Some things are intentionally open.  Some things are intentionally closed.  But more often, some things are accidentally open.  Or accidentally closed.</blockquote>

I do see some progress in libraries. More are demanding access to digital material for archiving and preservation in case the publisher goes poof. But don't forget where YOUR storing the data. If the data format, software, hardware or OS vendor goes poof, can you recover everything without loss?
