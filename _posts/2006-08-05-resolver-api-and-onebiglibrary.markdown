--- 
wordpress_id: 332
layout: post
title: Resolver API and OneBigLibrary
wordpress_url: http://blog.ryaneby.com/archives/resolver-api-and-onebiglibrary/
---
Dchud has a <a href="http://onebiglibrary.net/story/solving-the-appropriate-resolver-problem">nice post about using OCLC's resolver API</a> to integrate other institutions' resolvers with your application. The end result being that any user that comes across your site would be able to find it locally if they have an institution IP. One step closer to what I think Dan's OneBigLibrary idea might be. <a href="http://dilettantes.code4lib.org/">Ross</a> has also played with the idea in his metasearch/resolver and the idea opens some possibilities for users.

This raises the question in my mind about whether it may be worthwhile to proxy any link on a library site, even if it's a non-restricted site. May be at least worthwhile for links to digital libraries and open databases (oai, etc).

One of the things with dchud's implementation that didn't work as well is that it didn't use the text we set-up in the API and also didn't include the additional links. For some reason we have multiple resolvers listed and the first one isn't very useful (ILL) comparatively. We've since changed the order though so that should take care of that problem. As for the buttons, they do look nice but having the same text that FirstSearch and other sites use from the API may be less confusing. Just a few minor points.

If you developing some sort of repository or other database this may be something worth looking into. OPAC products would also be interesting. I'll have to bother Casey about including it in WPOpac.
