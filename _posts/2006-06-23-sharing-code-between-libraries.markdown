--- 
wordpress_id: 295
layout: post
title: Sharing Code Between Libraries
wordpress_url: http://blog.ryaneby.com/archives/sharing-code-between-libraries/
---
Awhile back I attended Library Camp and was lucky enough to have some dicussions with Alan Gray of the <a href="http://darienlibrary.org/">Darien Library</a>. It's a small public library that's doing it's best to stay relevant to the community. Some of the programs he discussed were quite inspiring.

One of his concerns was the technology side of things and that there was no way for his library to hire full-time programmers to accomplish some of the things other libraries, such as <a href="http://www.aadl.org">AADL</a> are doing. I threw out a few ideas such as companies like <a href="http://liblime.com/">LibLime</a> but that I would have to think about it more. It was a very difficult problem which is worth some discussion. I'm still not sure exactly what's best but figure I should throw out some of my current thinking to get things going.

The idea is to make software and other solutions created by libraries and reusable as possible so that other libraries can implement what's out there without reinventing the wheel or expending as much resources as the original. Let's face it, there are libraries that won't be able to do this sort of thing.

<h4>Vendor Abstraction</h4>

The first problem is the reliance on hacks. Many solutions are so dependent on library specific hacks that using them anywhere else would be nearly impossible. A possible solution to this would be the idea of abstracting the vendor layers as much as possible and use a standard input instead.

For example, I threw together a quick OpenSearch module based on the III XML Server. In hindsight it would have probably been better to build it on a standard layer and then make a library to convert from this standard to III XML and back. Some of the benefits:

<ul>
<li>Portable: Can be used with other vendor products presuming a library for the standard format is available</li>
<li>Vendor Proof: When the vendor breaks things (and they likely will) you don't have to worry about fixing the vendor code all over the place. You fix the standard library and the apps built on the standard then work. This isn't huge with just one module like OpenSearch but as you build more and more on top of the interface it becomes much more maintainable. You fix one class instead of 10.</li>
<li>More people can now contribute to the module itself. Instead of worrying about tweaking vendor-specific code, everyone can contribute back to the source, regardless of what they're running. This also helps with ports to other languages. The alternative is a module for each vendor also ported to each language.</li>
<li>Flexibility: Your library decides to change vendors? Change the standard library and your website/modules/hacks keep going. The change is no longer as much of a chore as it could have been.</li>
</ul>

So what should this standard be? I'm not sure yet. From talking to various people it seems like SRU/W is a good candidate for search-based applications. The data format? MARCxml seems like a likely candidate. There's still questions regarding holdings formats.

I got this idea from <a href="http://public.csusm.edu/dwalker/">David Walker</a> who <a href="http://public.csusm.edu/dwalker/shrew/">did a similar project</a> for likely different reasons. He needed a way to hook the INNOPAC into a metasearch product and that product happened to support SRU. I think it's fairly easy to build more and more on top of that.

Cons: An additional layer, performance, etc. I'm sure there are plenty but at this point I think the benefits likely outweigh it.

<h4>Open Source</h4>

I think it's very important that things created by libraries should be usable by other libraries. A major potential barrier to this would be licenses that prevent people from freely using it. I'm not sure what, if any, licenses would be the best for this. Some prefer GPL, others like BSD, Apache, etc. Probably a point worth discussing.

I'll again use <a href="http://liblime.com/">LibLime</a> as an example as I got the chance to talk to kados about it. LibLime is a company that supports open-source software in libraries such as Koha. They also do custom development of software that works on top of other vendor products. One of their requirements though is that the software they create on contract will be open-sourced so that other libraries (and liblime) can reuse what was created. I think this is a great idea. When a library that can afford to contract for an item has it created, all libraries benefit.

<h4>Community</h4>

I think community will play a large roll as it created a cheap form of help and support. Right now I think <a href="http://code4lib.org/">#code4lib</a> fills that role well. How well it would scale I'm uncertain, but it would be something to keep in mind. 

Documentation is also a roll the community can serve which some of use are doing for the III XML server, an expensive and poorly documented product.

<h4>Feedback</h4>

This is the first version of this idea and I will likely change my mind next week about it but please feel free to post comments or trackbacks with ideas or critiques.
