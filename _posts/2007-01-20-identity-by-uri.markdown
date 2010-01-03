--- 
wordpress_id: 443
layout: post
title: Identity by URI
wordpress_url: http://blog.ryaneby.com/archives/identity-by-uri/
---
There have been some great projects lately about moving information control into the hands of users such as <a href="http://www.movemydata.org/">Move My Data</a>. In that vein there is the idea of <a href="http://adactio.com/journal/1212/">profile data using microformats</a>. For example you have a list of your friends marked up on hcard on your blog. When you sign up for a social service then you just input a link to your blog and your friends are imported. And you can have subset's across services, giving you ease and control.

<blockquote>We donâ€™t need yet another centralised service. The information is already out there, it just needs to be explicitly marked up.</blockquote>

Decentralization and control by the user is also becoming important in the movement for "Identity 2.0". If you want a quick introduction then I recommend watching <a href="http://identity20.com/media/OSCON2005/">the OSCON keynote by Dick Hardt</a>. There are a few architectures that are being built around this idea but one that seems to be taking off is <a href="http://en.wikipedia.org/wiki/Openid">OpenID</a>. From the <a href="http://openid.net/">official site</a>:

<blockquote>OpenID starts with the concept that anyone can identify themselves on the Internet the same way websites do-with a URI (also called a URL or web address). Since URIs are at the very core of Web architecture, they provide a solid foundation for user-centric identity.</blockquote>

For those used to the normal user/password at every site it can be a bit of a hurdle to understand as it involves external providers and trust (<a href="http://en.wikipedia.org/wiki/Openid">from Wikipedia</a>):

<blockquote>Therefore, the strength of an OpenID login depends on how much a relying party knows about the authentication policies of the identity provider. Without such knowledge, OpenID is not meant to be used on sensitive accounts (banking, e-commerce transactions, etc.), but if an identity provider uses strong authentication, OpenID can be used for all types of transactions.</blockquote>

To help understand this here are a few posts you may find useful:

<ul>
<li><a href="http://apparentlymart.livejournal.com/2871.html">OpenID users can be just as trusty as local users</a></li>
<li><a href="http://simonwillison.net/2007/Jan/10/account/">An OpenID is not an account!</a></li>
<li><a href="http://simonwillison.net/2007/Jan/19/phishing/">Solving the OpenID phishing problem</a></li>
</ul>

If you'd like to get started learning more about OpenID or implementing it then here are some useful places:

<ul>
<li><a href="http://planet.openid.net/">Planet OpenID</a></li>
<li><a href="http://www.intertwingly.net/blog/2007/01/03/OpenID-for-non-SuperUsers">OpenID for non-SuperUsers</a></li>
<li><a href="http://www.intertwingly.net/blog/2006/12/28/Unobtrusive-OpenID">Unobtrusive OpenID</a></li>
<li><a href="http://sourceforge.net/projects/wpopenid">Wordpress OpenID Plugin</a></li>
<li><a href="http://www.myopenid.com/">MyOpenID</a> - free hosted provider</li>
<li><a href="http://simonwillison.net/2006/Dec/19/openid/">How to turn your blog in to an OpenID</a></li>
<li><a href="http://simonwillison.net/2006/openid-screencast/">OpenID Screencast</a></li>
</ul>

And for those in the library field that may think it's something to ignore, here's a nice post about <a href="http://efoundations.typepad.com/efoundations/2007/01/repositories_an.html">Repositories and OpenID</a> as author identity.

<blockquote>I've felt for some time now that any centralised approach to name authority is pretty much doomed to failure for all sorts of reasons that I won't go into here.  I've had at the back of my mind that one might be able to build a distributed solution using LDAP, i.e. based on the LDAP servers maintained by institutions.  But it seems to me that using OpenIDs has some significant advantages...</blockquote>
