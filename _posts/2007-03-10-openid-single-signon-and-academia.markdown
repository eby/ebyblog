--- 
wordpress_id: 489
layout: post
title: OpenID, Single Signon and Academia
wordpress_url: http://blog.ryaneby.com/archives/openid-single-signon-and-academia/
---
A ways back I looked into supporting campus authentication in some apps I was brainstorming and found the information rather lacking for our campus. It was also only IIS supported at the time which made me feel a little less secure about the whole thing. They now have an apache module and are working on single sign-on but I've scrapped any plans.

However, I am rather impressed by what CASE is doing. You can start by looking at <a href="http://wiki.case.edu/Central_Authentication_Service">a wiki page they have describing their system</a> and yes, the wiki even supports the CASE logins. You can also see that they have perl, ruby on rails, drupal, zope and other modules available. With choices like that I would not be surprised if their adoption rate is rather high.

What led me to the wiki was that they <a href="http://blog.case.edu/jms18/2007/03/09/openid_server_integrated_with_cas">now offer OpenID's for anyone with a CASE login using the single-signon system</a>. And from the posting:

<blockquote>And because it is integrated upwards towards CAS, it should interoperate with all of the other "identity systems/protocols" we've integrated with CAS like Shibboleth (and, in testing, Oracle's Single Sign On, Sun's, and Google's SAML-based Single Sign-On).</blockquote>

It's great to see people in academia playing around with identity and authentication like this. However, a commenter did point out the first thing that popped into my head:

<blockquote>Awesome! Will I have this OpenID forever, even after I graduate?</blockquote>

Here at MSU faculty usually keep their NetID and students have it for around two years after graduation. It will be interesting how universities and colleges handle this type of policy as people start linking their identity with the university itself. It's also a place that needs work for OpenID consumers. I've now lost the quote but someone made the comment that one of the crucial things missing is that consumers don't allow multiple ID's to be associated with an account, which would help prevent problems if one provider disappears, etc. 

Something to think about. And to academia, here is a nice example of central services and information that can be useful. Transparency and documentation is a wonderful thing.
