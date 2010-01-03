--- 
wordpress_id: 198
layout: post
title: When Bots Attack
wordpress_url: http://blog.ryaneby.com/archives/when-bots-attack/
---
No this isn't a post about our new robot overlords. It would not be wise for me to speak ill of them. In <a href="http://www.code4lib.org/irc/faq">#code4lib</a> there is a bot called panizzi that has a tendency of responding with random phrases whenever he is addressed. There are also various commands including one that allows you to speak through panizzi. While trying to debug some python a second instance of panizzi was connected to the channel under the name althea. I couldn't pass up the chance to see if they would talk to each other. Here is a transcript:

[16:48] &lt;panizzi&gt; althea: hello
[16:48] &lt;althea&gt; panizzi: Error: &quot;hello&quot; is not a valid command.
[16:48] &lt;panizzi&gt; althea: truncating at 30 chars
[16:48] &lt;althea&gt; panizzi: Error: &quot;truncating&quot; is not a valid command.
[16:48] &lt;panizzi&gt; althea: come again?
[16:48] &lt;althea&gt; panizzi: Error: &quot;come&quot; is not a valid command.
[16:48] &lt;panizzi&gt; althea: please tell me more about that
[16:48] &lt;althea&gt; panizzi: Error: &quot;please&quot; is not a valid command.
[16:48] &lt;panizzi&gt; althea: thankyou drive thr
[16:48] &lt;althea&gt; panizzi: Error: &quot;thankyou&quot; is not a valid command.
[16:48] &lt;panizzi&gt; althea: thankyou drive thru
[16:48] &lt;althea&gt; panizzi: You've given me 5 invalid commands within the last minute; I'm now ignoring you for 10 minutes.
[16:48] &lt;panizzi&gt; althea: @dict RTFM

Luckily there was a ignore statement or they probably would have flooded the channel.
