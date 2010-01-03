--- 
wordpress_id: 24
layout: post
title: Innovative XML Server - Documentation
wordpress_url: http://ebybox.aresgate.net/blog/archives/innovative-xml-server-documentation/
---
I've worked with a lot of Open Source software so I'm used to documentation that is lacking, but for a commercial product I have to say that the Innovative XML server has some of the worst I've seen. I've managed to create an OpenSearch module and RSS output (more details soon). To do this I was forced to study the DTD to figure out how to get all the data I needed. The documention did get me started as too some of the options but some of it was just plain wrong.

Here's a tidbit others might find helpful. The documentation states that if you want to get the IIIRecord portion of a result (includes holdings and ISBN,etc.) then you need to enter the following in the URL string:

noexclude=WXROOT.Heading.Title.IIIRecord

This is actually incorrect as the XML server is case sensitive. The actual code you need is:

noexclude=WXROOT.Heading.Title.IIIRECORD

I figured this one out through studying the DTD. There's some other things that caught me up. In order to use these options you need to make sure there is no trailing slash on the URL. For example:

path.to.xml.opac/tgenetics/0/0/1/1/?noexclude=WXROOT.Heading.Title.IIIRECORD

will not return anything, but the following will:

path.to.xml.opac/tgenetics/0/0/1/1?noexclude=WXROOT.Heading.Title.IIIRECORD

Notice that there is no slash after the last "1". The documentation is vary scarce on examples relating to the urls.

Something for those working on similar things. More information on how to make RSS feeds, etc soon. I'll get into my problems with the schema as well.
