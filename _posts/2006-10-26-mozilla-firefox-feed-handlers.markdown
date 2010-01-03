--- 
wordpress_id: 401
layout: post
title: Mozilla Firefox Feed Handlers
wordpress_url: http://blog.ryaneby.com/archives/mozilla-firefox-feed-handlers/
---
One of the nice features of Firefox 2.0 is that you can assign other applications to be your feed handler (when you click the feed icon in the address bar) including web-based ones like Google Reader or Bloglines. I personally use a local install of <a href="http://gregarius.net/">Gregarius</a>. The latest version out of SVN has a button to register your install as a handler, but in case your wondering there are a few ways to add a custom handler (<a href="http://forums.gregarius.net/comments.php?DiscussionID=455">from the Gregarius forums</a>):

First you can <a href="http://developer.mozilla.org/en/docs/DOM:window.navigator.registerContentHandler">create a javascript based link</a>. This will make it easier if you have people who use your application or site.

Secondly you can create some preferences (strings) in the about:config area where # is a number that is not already being used by Firefox and the URI part is the subscribe url for your web application (%s is where the feed URL will go):

<ul>
<li>browser.contentHandlers.types.#.title = My News Reader</li>
<li>browser.contentHandlers.types.#.type = application/vnd.mozilla.maybe.feed</li>
<li>browser.contentHandlers.types.#.uri = http://yoursite/url=%s</li>
</ul>

I had to restart Firefox to get it to show up in the preferences. The third way is even more involved and requires editing the user.js file in your profile directory. You would add the following lines:

<ul>
<li>user_pref("browser.contentHandlers.types.#.title", "My News Reader");</li>
<li>user_pref("browser.contentHandlers.types.#.type", "application/vnd.mozilla.maybe.feed");</li>
<li>user_pref("browser.contentHandlers.types.#.uri", "http://yoursite/url=%s");</li>
</ul>

Again thanks to the people in the <a href="http://forums.gregarius.net/comments.php?DiscussionID=455">Gregarius forums</a> for pointing this out.
