--- 
wordpress_id: 477
layout: post
title: Transcript of Dan and Jon's Podcast
wordpress_url: http://blog.ryaneby.com/archives/transcript-of-dan-and-jons-podcast/
---
As I'll be having a long drive/ride down to Code4Lib this year I decided I'd try out the <a href="http://castingwords.com/">CastingWords</a> service for transcribing podcasts. I tend to prefer to read over listen. Once podcast I'd like to catch up on is the <a href="http://blog.jonudell.net/2007/02/16/a-conversation-with-dan-chudnov-about-openurl-context-sensitive-linking-and-digital-archiving/">OpenURL talk by Jon Udell and Dan Chudnov</a>.  Both Jon and Dan have agreed to let me post it publicly, so here it is for any others who prefer to read. Thanks guys!

I can attest that the CastingWords process is pretty nice. They seem to have done a good job from a glance through (I haven't read it yet) but then I haven't listened to the original. But if they manage to get "COinS" right then there must be something good going. So without further ado here are some downloadable versions:

<ul>
<li><a href="http://blog.ryaneby.com/wp-content/21803.html">HTML</a></li>
<li><a href="http://blog.ryaneby.com/wp-content/21803.txt">TXT</a></li>
<li><a href="http://blog.ryaneby.com/wp-content/21803.rtf">RTF</a></li>
</ul>

<h2>A conversation with Dan Chudnov about OpenURL, context-sensitive linking, and digital archiving</h2>

<div id="transcript">

  <blockquote class="speaker_1_text">
 
  <cite class="speaker_1" >Jon Udell:</cite>      

Hi, this is Jon Udell. My guest for this week's podcast is Dan Chudnov. He is a programmer who has worked on library information systems at MIT, at Yale, and soon at the Library of Congress, where he will be starting a new job shortly. This conversation is kind of a sequel to an earlier one with Tony Hammond of Nature Publishing Group. Tony talked about how digital object identifiers are being used in the world of academic publishing to create a stable, long-term framework for persistent linking and reliable citation.

There is a related technology called OpenURL that plays a role in academic publishing, but it is also something that Dan Chudnov are approaching from the perspective of libraries, that need citations to be not only durable and persistent but also to be able to redirect into the holdings of a particular library. It all sounds kind of esoteric, and in a lot of ways it is, but these questions of digital archiving and persistent linking will matter more and more, because we are all creating the library of the future.
</blockquote>

<blockquote class="speaker_2_text">
 
  <cite class="speaker_2" >Dan Chudnov:</cite>
      Hi Jon, how are you?
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      I'm good. I gather you have moved to my alma mater?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      No, actually, I come from there. I have had that address for like 16 years.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Oh, OK.
  </blockquote>
  
  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      I got both of my degrees in Michigan.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Oh, but are you not at Yale now?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      I am between jobs, literally. I have been working at Yale for a while, and I am actually about to start a new job in a few weeks.
  </blockquote>

  <blockquote class="speaker_3_text"> 
  <cite class="speaker_3" >Jon:</cite>
      OK.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      I am going to be working at the Library of Congress starting the first week of March.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Well, good for you!
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Thanks.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      What will you be working on?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      There is a new-ish unit there called the Office of Strategic Initiatives, and in that unit there are a number of software development groups, and I will be on one of them. This group is tasked with building, buying, selecting, implementing new systems for other parts of the library. That is a pretty broad scope, but I think most of what they do right now is building digital repository systems.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Sounds like the perfect thing for you.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Well, I hope so. We'll see.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      So, you'll be moving to Washington.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes. It's a big move, because we have been in New Haven for--I have been here for 10 years, my wife has been here for about 12 years. But it is an exciting job; the door is kind of wide open it seems.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Well, good for you. I was thinking about how we should frame this, and it is a challenge...
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes, it is, isn't it?
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      ... because first of all, you operate in this domain of folks who call themselves &quot;library geeks, &quot; and I tend to operate in this domain of folks who call themselves &quot;general-purpose geeks, &quot; and there is much translation that needs to go on even just between those two realms.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      True.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      But the larger and more difficult translation that needs to go on is sort of to everyone else, as to what the heck is any of this stuff about and why should we care?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes.
  </blockquote>

  <blockquote class="speaker_3_text"> 
  <cite class="speaker_3" >Jon:</cite>
      That is quite a challenge for us, but still I think we should try.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      OK.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      What I had hoped to do here was kind of a follow-up to the conversation with Tony Hammond, where we dived into the entrails of the Digital Object Identifier system.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Right.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      I was trying to relate that to a general problem that everybody has, and I think that is completely valid, which is that we are all increasingly in the situation of needing to care about this question of the persistence of our digital artifacts, which we have more and more of all the time.
      
      Why don't we kind of start there, from the perspective of the various library-related linking and resource-identification standards that you have been involved in. So if you could sort of back up and state the problem first, in a way that everyone could relate to, that would probably a good place to start.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      OK. Well, Tony certainly is eminently qualified to speak on these things, and I really enjoyed your conversation. He has had his hands in and been a member of committees and things, and I have done less of that. I have been more of an informal participant in standards, so what you will get from me is a little bit more of the casual, library employee view of a lot of these things, so hopefully that will be practical in another way.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Yes.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Well, should we start with names or should we start with the storage and preservation questions?
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Well, maybe we should start with the perspective that someone has who is on the Web and runs into this funny-looking thing called an OpenURL.
  </blockquote>

  <blockquote class="speaker_4_text"> 
  <cite class="speaker_4" >Dan:</cite>
      Well, sure.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      And talk about sort of what that is, what it's doing for me, and why.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      The further I get into this, the more I like to frame things as really old questions, just reappearing. The problem you are trying to solve when you run into an OpenURL is really an old problem, it is as old as research itself, and that problem is to follow the history of thought in a problem space, when you read someone's article and then relate it to work that has come before.
      
      You want to be able to follow the references, essentially, and see which giant's shoulders they have been standing on, and verify that these people are building on the right combination of work when they are proposing a new idea or a new solution to a problem.
      
      Part of that is simply verifying that their statement of problem is accurate and they know what they are talking about; and the more important probably, progressive aspect of that is being able to verify scientific results and claims. So you need to be able to follow people's references if you want to do science.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Sure, and obviously everything changed when we got the ability to turn footnotes into things that actually went someplace in real time. That was amazing, it still is amazing.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes, absolutely. And this problem is not just as old as footnotes and academic journals, which are several hundred years old. It is also, more to the point, it is as old as computing. Garfield and his work with ISI, analyzing citation results, dates back more than 50 years. So as long as there have been computers to help with this kind of thing, there have been people who are ready to do this kind of analysis.
      
      Basically, what you want to be able to do if you are reading an article online, much like you would want to do if you have a physical copy of the paper, is when you are looking at the references you want to go and follow those references. You want to find which journals, which issues, which volumes, which pages these references people are citing, are relevant to your understanding of the problem you are trying to understand with the author's perspective.
      
      So, you literally need to go into the book stacks, the journal stacks, whatever, and find that volume, that issue, that page of that journal, so you can find the article, and this is exactly the problem as it translates to the Web that led to the development of the OpenURL standard seven or eight years ago. That problem is, you are using an online article, you are reading an article in an online journal, and at the bottom of the article there are a bunch of references.
      
      And the references aren't homogeneous in any way, in the sense that, well, they are probably formatted the same way visually, and there are obviously styles people use to keep that consistent--short form of the author's name, and a title of the article, and a short form of the journal title, and reference to volume, issue, year, page--but that is really hard to translate mechanically online for a couple of reasons. One is that metadata, first of all, is very sloppy. Author names are ambiguous, journal names can be ambiguous, journal names change every time journals split. Book titles are mistyped, misquoted, that sort of thing. There is a lot of slop in the system.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      So, hang on just a second, let me back up and ask kind of a naive, devil's advocate question. Assuming that the article that you want to read online has been published by someone, somewhere, online, it will have been published at a URL, and you don't care, shouldn't need to care, what is contained in that URL. It is just an opaque thing that you click and--bingo!--you go to the article, right? But obviously there is more to the problem.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Right.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Especially in the case of libraries, especially in the case of holdings which are accessible to library patrons or someone at a particular university, so there is this question of getting redirected to your local copy of the thing that you are allowed to read.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Exactly. That is really where they were starting to solve the problem here with the OpenURL. What people working in this area recognized immediately was that any particular library, particularly a big research library, is likely to have subscriptions to most of the kinds of journals that most people in a certain field would be looking for; but the journal subscriptions themselves, although they are all online and the articles are all published online--and of course, that is actually very new.
      
      If we go back six or seven years that wasn't necessarily so at all. This is all actually very recent, that you could assume that most recent things would be online. But they are all published by different publishers, and the different publishers maybe publish the journals themselves on their own sites, or they contract with third parties to publish them for them in their own systems, or there are gateway systems that essentially aggregate resources from a variety of publishers into whole new interfaces.
      
      And when you are working at a big library like Yale University's libraries, not only are you going to have an unholy combination of all these subscription agents and aggregators and source publishers themselves subscribed to in your library, but the resources themselves are going to overlap.
      
      So, when you follow a reference link, what you need to know is whether you have that journal at your library, and not just whether you have that journal, but which system you can use to get to it, and within that which of those systems actually allow you the specificity of naming a volume, an issue, a page, an author name, a unique identifier, and can get you right to that article itself.
      
      What you really want to be able to do is bring people right to the full text of the article with one click. Unfortunately, with all these reasons, it is just not always that easy.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      It seems that there are a couple of different things going on here. In one case, the need for an intermediary would be obviated, if we were in an open access regime and there was a canonical <a href="http://archive.org/" >archive.org</a> URL for, let's say, a math article or a physics article. Then it is not going to be a question of needing to get redirected to my library's copy of that thing, because we can just use the canonical copy, right?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      In theory. That is the sort of thing that works in the short term in reality, in our experience. Resources move. If you watch even the history of individual publishers who have been online since the early days of the Web, and you follow the URL patterns that lead to articles at their own sites, and remember every system upgrade they have gone through, and every time they have overhauled the Web back end and replaced it with a new one, even if there were some single site that tried to preserve some sort of links, from the perspective of a librarian you kind of have to assume that even they will change their linking structure over time.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Even <a href="http://archive.org/" >archive.org</a>.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Sure, although <a href="http://archive.org/" >archive.org</a> isn't really organized to provide this kind of access. Secondarily, <a href="http://archive.org/" >archive.org</a> is not an arbiter of which resources a particular library has subscribed to, so whether or not you can get to the links is independent of whether you as an individual, working through your institution or maybe independently, have rights to see what is behind the link. There are all these things that can come up and cause problems.
      
      The identifier aspect of this is one big step in mitigating some of these issues, because if you have a known, unique identifier, you can recognize that as such and have a little more mechanical strength in trying to resolve it to a direct link. A lot of what you talked with Tony Hammond is in that space.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      So, the DOI being an example of such an identifier.
  </blockquote>

  <blockquote class="speaker_4_text">
 
  <cite class="speaker_4" >Dan:</cite>
      Yes. Other obvious kinds of identifiers are URLs in general, and PubNet identifiers if you are in a medical space, like I have been working in most recently. These are well-known, they are well understood, they are easily recognized, and they are usually fairly easily resolved.
      
      Now one of the jobs I have had in a previous life was I was wondering on the D-Space project at MIT Libraries about six years ago, and even just the &quot;how to generate IDs and resolve identifiers&quot; problem alone, on that project, was a source of endless debate, and not even... What we came up with isn't even necessarily something that pleases all parties all the time.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Well and apparently it has changed over time as well, right?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes, it has, I think. And different institutions have chosen to implement it differently.
  </blockquote>

  <blockquote class="speaker_3_text"> 
  <cite class="speaker_3" >Jon:</cite>
      So, for example, Tony was saying that initially the recommendation was to make them completely opaque and not intending to be meaningful to humans, but then eventually people realized that was a bad idea and there should be some human readability in the identifier.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Well, what you really want to be able to do is recognize identifier patterns, at least. If you see something with a PMID in it, and it is structured in an URI, which is another effort Tony was involved in developing, then you can predictably figure out what that is.
      
      With the D-Space project, one of our exclusive goals was to solve this, and in many ways to support open access publishing by making it easier for authors and institutions to publish their own words by, as much as anything else, not only taking a copy of the content and offering to manage that over time, but also simply offering a stable URL.
      
      If you talked to a number of authors at MIT five years ago, they would line up right away and tell you that, sure, they had been publishing their own articles, but their graduate assistant system administrator had moved on, and the system had been compromised, and now the links don't work, and they have been publishing papers and now no one could get to their articles anymore. &quot;Yes, please take a copy of this for me and give me a stable URL that I can cite.&quot;
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      So in response to the thing that Tony and I did, a number of people pointed out that there are any number of ways to materialize a persistent URL, and ultimately there are certain technical questions about how you manage that process, but really it comes down to governance and infrastructure and a business model that enables that to be sustained over time.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      That's true. You can think about that in a very kind of centralize, monolithic way, like, &quot;What if there were one organization whose job it would be to do this?&quot; Or you could think about it in a very distributed way, and being a librarian this is the way we tend to think about it. We all have different libraries because there is this nexus of need, in a given institution, to centralize some of those responsibilities for a specific community.
      
      So in this particular sense I think there is an importance to the role of needing some sort of distributed identification resolution stuff, because if all the libraries put their eggs in one basket, with one centralized service, and then anything happened to that one centralized service, that is a traditional single point of failure problem: we simply can't provide the service we need to our communities. So negotiating this spectrum of what you need to centralize, what you need to distribute, is an ongoing and fairly difficult process.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Right, but it is also the question of whether you consider any given implementation of this idea. So let's take the DOI handle stuff, for example. In one sense it is a decentralized system in that there are going to be multiple handle servers and resolvers and so on.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Right, and you distribute the naming authorities as well.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      And distributed naming authority. But in another sense, it is kind of a single thing in the sense that it is somebody's business to run that.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes, absolutely. And in practical terms, the way it has been implemented is that it is almost entirely done through a single resolution step, through the organization whose responsibility it is. Most people who implement handles--now, of course DOI is an application of the handle system as well, that has its own back end--but handles in general, if you were to get a copy of the handle system CNRI, and run it, and start assigning handles in Microsoft for your documents, you would either need to make a choice to use the centralized handle system to resolve those http projections of handle identifiers into the public Internet, or you would need to implement your own systems to do that. And that is exactly the same centralized/distributed question all over again.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Right. Right, it is confusing.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes, it is very confusing.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      It's not just me.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes, but it works great. It is a huge improvement, but it doesn't necessarily clean everything up all tidily. And of course, organizations are bought and sold. Not that we expect Microsoft to be bought or sold anytime soon, but organizations change over time certainly, as well, and missions change, and they merge, and they split, and they die. When you are trying to deal with the long term, these questions inevitably come up.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      This feels like a replay, to me, of another debate I have been having with myself and other people. So, for example, in another context, the question about social networks and the multiplicity of social networks...
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Good question, yes.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      ... versus the overarching, if you want to call it, social network which the Internet potentially is. I can look at these various schemes for URL persistence and decentralized networks that support that idea as a bunch of contenders for something which is ultimately wanting to be rolled up and simply be part of the fabric of the Internet.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      In a way that it isn't already?
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      In a way that it isn't already, yes. So for example, what we don't have as part of the fabric of the Internet is both a technical infrastructure and a governance infrastructure in support of archiving and preservation and persistent reference. It is just not a property of the Internet itself. So we are creating it in a variety of add-on layers, which to an outsider look like a confusing landscape because they are both, in some ways, I guess competitive but also overlapping.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Well, in one way you could look at the brilliance of the HTTP specification and the model for URIs and URNs and URLs and say, &quot;Well, they have enabled us to build that, but haven't really specified all the details about how and why to do that.&quot;
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Right.
  </blockquote>

  <blockquote class="speaker_4_text"> 
  <cite class="speaker_4" >Dan:</cite>
      Another way to think of it--and I guess this is something else I wanted to say about OpenURLs--is, in this case I think what is really happening that is always going to complicate things is you are not just crossing between user interfaces and machine interfaces, but you are inevitably crossing into &quot;meet space, &quot; and you are dealing with individuals who are not in front of their machines, and physical media that are not connected.
      
      And that is certainly the problem we can't ignore in libraries, and on that level we have hierarchies of authority and responsibility, from individual responsibility to organizational affiliation to networks of organizations; and in a sense this tapestry that is building out on the 'Net, this thing that is missing, is approximating the complexity of &quot;meet space&quot; that in some sense then maybe it is fully built. In another sense, maybe the tapestry doesn't work unless there are clear overlaps and interconnections between.
  </blockquote>

  <blockquote class="speaker_3_text"> 
  <cite class="speaker_3" >Jon:</cite>
      I actually thought where you were going with that was to point out that the DOI, for example, was a really concise token that can be printed at the end of an article, and is a small number of characters that someone could actually write down on a three-by-five card and take away with them.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      It's true.
  </blockquote>

  <blockquote class="speaker_3_text"> 
  <cite class="speaker_3" >Jon:</cite>
      I thought that was actually a pretty important property.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      I wouldn't dispute that at all. But would you put a DOI on your business card?
  </blockquote>

  <blockquote class="speaker_3_text">
   <cite class="speaker_3" >Jon:</cite>
      I don't know. What would it point to?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      That's a good question.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Yes. But there is an interesting contrast there, in fact, which I wanted ask you about, to sort of get back to OpenURL. An OpenURL, as I understand it, looks more like query. So I am looking at one example of an OpenURL here, and it has some resolver domain name and then there are a bunch of named value pairs: article title, volume, issue, date, page, journal title, ISSN, and so on, right?
      
      So, in fact, what it looks like happening here is, it seems very similar to what Tony was describing as the query process, going into the DOI and handle stuff, where you want to get back a concise identifier, but you need to ask the system, &quot;What would that be for these values?&quot; Is that a fair statement?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes, it is. The way the standard is written, unfortunately, it is a little too complex. I am both a huge fan and a huge critic of the OpenURL standard itself. What they are describing is a framework for context-sensitive linking, and what they mean there is that for any given bibliographic object you are referencing, you want to do exactly what you just described. You want to run a query for the services that are available, that are available to me, through my institution, for this object; and hopefully what most people are doing most of the time is they are trying to find a full text link.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Right.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      So, in that scenario, whether or not you find an identifier, per se, isn't of primary importance. If an identifier comes with the query it is helpful in locating the resolution step--which resource is going to have a copy of that--and getting you precisely to the copy of that you want. The trick, though, is you might not just want to find full text. What you might really want to do is save a reference to this.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Right.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Or you might want to do a cited reference lookup, and then you might want to do an interlibrary loan request if you find through the system that you don't have a copy. The way most OpenURL resolver systems work, in the thousand or so libraries that are using them, is query results in a human interface, offering options.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      OK.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      If at all possible there is a physical link, whether it is through an identifier and a system like DOI or not, and usually it is going to take you right to an article--usually it is going to be an article. That should be first. Typically, at a place like Yale, for the highest impact factor journals, you are going to get several options for the same journal. You are going to be able to go directly to a publisher's site.
      
      You are going to be able to go to an open-access copy of it. You are going to be able to go to an aggregated version of it in something like Lexus-Nexus, Academic Universe, that kind of resource, or a gateway subscription service like EBSCL. So you might get several copies of links that are all different, that are all going to take you to versions of the article; and below that you will get links to an interlibrary loan service if you aren't lucky about that.
      
      Now, another project I have been working on, and some other people in the community are trying to improve the step, is basically what you are doing is, not only are you presenting users who typically just want to get right to the full text with this confusing screen offering these options in the middle of which is the full text link, so just take me there darn it. You are also, you are moving users through three different systems at once.
      
      For every reference you want to follow, you need to come up out of the silo of content you started in, which might or might not be the same one you have to go back to a month later to get to the same article; step through the library's user interface; remember how to follow the links in there; and end up at the ultimate site, which might be, again, different from one month to the next depending on library subscriptions, which come and go and change over time as well. And that is really confusing.
      
      Every time one of my colleagues has reported to me, informally or more publicly, on usability testing results from OpenURL screens, the result is almost invariably, &quot;I think I know from this that if I click the first thing I will get to the full text, and I remember seeing it, so I do that.&quot; But they don't read it, they don't remember the different options, because these screens are typically just not that good yet. They need a lot of improvement.
      
      So, a project I am working on now, I have been consulting on this effort called LibraryFind, a metasearch project coming from the Oregon State University Libraries, funded by the State of Oregon. It is a metasearch tool which allows you to search multiple resources at once. We have basically embedded an OpenURL resolver into the result stream, so that when you do a search on someone's name, like yours, or a topic or the name of a book, hopefully what you are going to get are not just links to OpenURL resolver screens--we control the whole system, right? We have got these front-end-to-back-end searches that are licensed resources; and we have got the OpenURL resolver; and we have the knowledge base of which resources were subscribed to.
      
      So, what we are trying to do is reduce it to two clicks. You send your search query to find what you want, and if we can find a link directly to full text we are just going to give you that link right away in the results. So one click to find, one click to get. And when we have done usability testing on this, it is amazing. There is no question what it does. People instinctively want to just click on the result and get the full text of the article when you are doing article searching.
      
      And when we are able to provide that, which is in many cases, people don't even recognize what is happening, because the number of systems they have moved through has been reduced and the number of screens we were confusing them with has gone down.
      
      Of course, this doesn't always work. If you are doing book searching, you are trying to find a book, you are not necessarily going to find an e-book copy. So then we have to move you through data from the online catalogue, and figure out if it is online, and figure out where it is on the shelf and whether it is checked out. These problems just don't go away; there is always a possibility for great confusion. But we are trying to find ways, both through this project at Oregon State and a lot of other initiatives going on, to shorten these steps.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      From a person's perspective who is using a system that is instrumented this way, there is the question of, what is the query that I formulate? The OpenURL, although they probably don't interact with it directly, is a way of formulating that query, right? So I know the title and the author, I will put in that much, and will hopefully get back a result set that I can scan and then, as you described, through this interactive step, I can refine that.
      
      But on the other end of it, I want to cite this thing, and I want to cite it in a way that is canonical and durable. So, at that point, what does that part of the process look like? Where do I end up with the OpenURL that I want to point other people to?
  </blockquote>

  <blockquote class="speaker_4_text">
   <cite class="speaker_4" >Dan:</cite>
      Yes, OK, so that's a tricky question, again for a few reasons. One is that when somebody puts through an OpenURL query, you might or might not have a robust, accurate, set of metadata in that query. If you have an identifier or you have some complex matching, you can restore metadata into that transaction, much like--you know, there is this great book by Daniel Hillis, &quot;The Pattern on the Stone,&quot; where he talks about the ways you can build complex CPUs with Tinkertoys or something like that, but over time that noise gets into the system because of the realities of physics, and you have to essentially provide redundancy so you can restore the logic at any point where the logic might have been corrupted or lost some signal.
      
      And essentially what needs to happen at that moment is we need to restore metadata, we need a restoring metadata system; and in some cases, certainly when you have things like a reference object that you are passing by reference with an identifier, you can do that fairly reliably. If you have some combination of fields like title and author and pages and publication date, it's a bit more of a crapshoot. But if at all possibly you do want to be able to restore that full record, and in addition to providing a service which would lead people to full text, you do want to provide a canonical citation form.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      What would that look like?
  </blockquote>

  <blockquote class="speaker_4_text"> 
  <cite class="speaker_4" >Dan:</cite>
      Well, I think one system that has implemented this is the O-Link system, which a group in OhioLink has done this for libraries across the State of Ohio. I think what they have done is, literally the text string that you would want to use if you would want to cite this reference in your paper.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      And how would that look?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Well it is back to what we see in printed journals. It is the short form of the author name, a title, volume, issue, page, journal name, and date.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Oh, OK.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      And that's great. But immediately, then, you start thinking about--and this gets back to social bookmarking and all of that--you want to do the kind of thing that Tony and his colleagues at Nature have done Connotea. You want to be able to share this thing. That was how I discovered social bookmarking. We were already using OpenURL Systems, and in about 2003, at this fun conference I go to every year in Canada called &quot;Access&quot;--we do this thing called &quot;Access&quot; where we take suggestions for wacky ideas and we work on them for a day, just to get our minds around new technologies and work with each other and have fun.
      
      We thought about what it would like if you could just track a community's OpenURL resolutions, and just have a stream that would show up, and a feed you could subscribe to, of all the references people are going to over time. And in a lot of ways this is what social bookmarking is: you are reading over people's shoulders, you are seeing what your friends are reading.
      
      What I think hasn't happened yet is for those two areas of functionality to really be bridged. I don't think there is an OpenURL resolver on the market that not only provides full text links and a citation form but also automatically lets you save a resulting citation into a community bookmarking service.
      
      But thinking about those issues led us to this other generic problem, which is, &quot;Well what if I'm--well, I'm working at Yale, which is lucky for me, I'm lucky to be there and they have great resources; but if I'm writing a paper and want to publish it on the 'Net, and I want to blog about it, how do I put up OpenURL links that other people can follow? This is a huge problem.
      
      We have come up with a temporary solution to that. Again, it is another community initiative, and this one is called COinS.
  </blockquote>

  <blockquote class="speaker_3_text"> 
  <cite class="speaker_3" >Jon:</cite>
      OK, I've seen it.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      COinS is awkward for all the reasons that OpenURL is awkward, but it is also very simple in that it is a way to specify an OpenURL in a SPAN tag in HTML. It allows you to disconnect the user and the publisher, so that there is no presumption of knowing where the user is coming from, and for the user visiting a blog entry with a reference in it, there is no presumption that the person publishing the link is assuming that you should go to some specific publisher's site, because you might want to go somewhere else.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      So, in other words it takes the resolver out of the equation and just packages up the raw metadata that would be the query that would retrieve the article?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Exactly that, and it does that using the exact terms of the most common formats for referencing articles and books from OpenURL.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      So, then you would need a companion piece of software that would attach to your local resolver.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Right, which is both great and a problem. It is great because it opens up this opportunity for Bookmarklets and Greasemonkey scripts, and we have all been through that and it works great. We have done is we came up with a simple way to activate a COIN. See, COIN stands for Context Object In Span, &quot;Context&quot; being the part of OpenURL that specifies this metadata package that you are sending over the wire, and &quot;Span&quot; being the SPAN tag in HTML. It is essentially like a micro format. We were working on this before we knew about micro format. Maybe we would have tried to consolidate all the terms, I don't know. Basically it is a micro format-like convention for putting your context object into a SPAN tag.
  </blockquote>

  <blockquote class="speaker_3_text"> 
  <cite class="speaker_3" >Jon:</cite>
      How would you format, then?
  </blockquote>

  <blockquote class="speaker_4_text"> 
  <cite class="speaker_4" >Dan:</cite>
      Well, you can format by hand, of course. That's kind of a pain. There are a couple of sites on the 'Net that will allow you to generate one. I think the division of OCLC called Openly Informatics has a COinS generator that you can use. I don't know if there is a web service to that or not, but it would make sense that there would be. So you can basically send it terms and it will give it back to you.
      
      There are also blog plug-ins. I think there is one for Re-Press.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Oh, yes?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      We have also worked on one using the structured blogging tools, if you are familiar with that. If you download that stuff, one of the bundled reference types is a journal, and another one is a book. If you just type in a few fields for title, author, journal name, publisher name, and a date, your volume, issue, pages, all that stuff, for an identifier, it will generate a COinS for you. Of course, those aren't necessarily widely used. There is a huge step with being able to publish it there. But hopefully that simplifies some of it, and we have found a few of these on the 'Net.
      
      The problem, then, goes back to, how do you give people this thing they have to install? I mean, what we are learning is if you make people install something, they won't do it unless it comes with... you know, if you get Microsoft Office Suite or Firefox. If it is not something that is right there and one click away, it is not something people are going to find on their own.
  </blockquote>

  <blockquote class="speaker_3_text"> 
  <cite class="speaker_3" >Jon:</cite>
      Exactly.
  </blockquote>

  <blockquote class="speaker_4_text"> 
  <cite class="speaker_4" >Dan:</cite>
      So fortunately there has been some more work done on this. OCLC has what they are calling the &quot;OpenURL Resolver Registry.&quot; They have collected records from over 1,000 institutions of where their OpenURL resolvers are, what mechanisms they support, what the links to them are, what the icons you want to display for them are, what the short, catchy local title of it is--whether it is GetLinks, or Yale Links in the case of Yale, or GetIt or FindIt, whatever it is. It varies across institutions.
      
      And what we have done, I have worked with them to produce a simple database of Greasemonkey scripts and Bookmarklets for all the institutions in that registry, so that librarians can go and get one of these things and distribute it on their campus.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      OK, I think I have seen that actually.
  </blockquote>

  <blockquote class="speaker_4_text"> 
  <cite class="speaker_4" >Dan:</cite>
      Yes, and that works. There is no denying that it works. People are publishing COinS and there are some sites that are fairly visible that are publishing COinS now including <a href="http://worldcat.org/" >WorldCat.org</a> and Wikipedia, and some work has just been done in Wikipedia to actually improve the quality of COinS coming out. So anytime the standard Wikipedia citation templates for journal articles or books are used, a COinS is going to come out.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      So let's walk through this, because a Greasemonkey script or the equivalent in IE is kind of a non-starter for most people. A bookmarklet is problematic but at least more broadly accessible. So, assuming the bookmarklet, what would be the flow here? How would this work?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      As is the problem with any bookmarklet, you have to go and get it and install it. You need to find the one for your institution.
  </blockquote>

  <blockquote class="speaker_3_text"> 
  <cite class="speaker_3" >Jon:</cite>
      Right, but assuming you have gotten that.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes, if you have gone and done that, if you have got it sitting in your toolbar, whether you are in IE or Firefox or Opera or Safari, if you are on a page that has references you would be presumably intelligent enough or experienced enough to know that if you clicked that, you might find links back from references to your own.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      But the page would let you know that it had stuff that would be activated by that bookmarklet?
  </blockquote>

  <blockquote class="speaker_4_text"> 
  <cite class="speaker_4" >Dan:</cite>
      We don't have a convention for that. Of course, if you are using the Greasemonkey form it will just pop up automatically and you will see the link. If you are using a database that you are familiar with, you will probably learn that you can try clicking your bookmarklet. This is an area of usability where people don't necessarily get it right away, but we typically have repeat users. Whether someone is an undergraduate or a faculty member, they are around for a few years. After a while, you get to know the databases you are using and you recognize the patterns.
  </blockquote>

  <blockquote class="speaker_3_text"> 
  <cite class="speaker_3" >Jon:</cite>
      Some other page has references that are encoded as COinS, which are these micro formatted thingies inside of expand to x, and I click the bookmarklet in order to do what, what happens now?
  </blockquote>

  <blockquote class="speaker_4_text"> 
  <cite class="speaker_4" >Dan:</cite>
      Little icons that point back to your institutional openURL resolver will show up in the page.
  </blockquote>

 <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      OK.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      That kind of headless server name lists COinS tags, which are basically context objects not bound to a specific resolver on the net...
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      OK.
  </blockquote>

 <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      ...are turned into additional anchor links with an HREF that is a fully formatted openURL link that takes the context object it found in the COinS and binds that to your institutional resolver. Hopefully, pops up the icon for your institutional links and a little short name of it.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      So this is on the reading side, if I'm writing something, in particular, if I'm writing something for the web, is there even a procedure available that would enable me to form some sort of openURL enabled link that I could publish out to people who would then resolve it, wherever they happen to be.?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      If you're writing your own system, and you're going to be doing a lot of this, it's fairly easy to tweak your user interface template and push your metadata into a coin span tag. That's straight forward, if you had the metadata in hand, if your system is robust enough to have these fields delineated, you can just follow the convention and publish them that way.
      
      If you're a blogger, you're going to want to rely on one of these things like the WordPress plug-in or the Structure Blogging plug-in for removable type or Drupal.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      And you can configure those to work against your local catalog?
  </blockquote>

  <blockquote class="speaker_4_text"> 
  <cite class="speaker_4" >Dan:</cite>
      You can, both publish your own openURL links and your own posts that by default go to your institution, particularly, if you're writing web logs for your own institution. But there is no reason you can't co-publish that with open COinS. So that people who come to your weblog they might see a Yale link, but if they recognize that, they might click their bookmarklet and find, say you have one running at Microsoft, if you have a Microsoft resolver you can have a bookmarklet for your Microsoft resolver and follow that into the Microsoft research lab.
  </blockquote>

  <blockquote class="speaker_3_text"> 
  <cite class="speaker_3" >Jon:</cite>
      I think, I'm starting to get the picture here.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      It's not a clear picture, I'm sorry it's kind of confusing.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      I understand, so in principal, I could be a blogger who is intending to bridge between the realm of academic discourse and the realm of public discourse in the blogosphere and could do so by using some sort of plug-in that would present me with a form into which I would place partial information about a resource, an article, and would get back a completed version and would get it back in a form, but one of which would be this COinS thing which could be embedded into my blog posting which then could be interpreted by a COinS interpreter or resolver or client, whatever you call it, by someone somewhere else.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Right. That would be a useful service, and I think I mentioned, I think that OCLC has a COinS generator, that you can find off the main COinS page at <a href="http://ocoins.info/" >oCOinS.info</a>.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      My following question here, for some reason, I've been deeply vexed by this question. This doesn't seem to bother most people, but I worry a whole lot about the way in which, in the blogosphere, we are able to know who is paying attention to which resource, by looking at sites like <a href="http://del.icio.us/" >del.icio.us</a> and Technorati to see who's been linking to or pointing to this thing, but the thing, the referent, is very sensitive, even case sensitive.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes, I read your post about that recently.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      From the standpoint of aggregating the attention that flows to a resource. We have systems that, on the one hand, work remarkably well, really. When you think about it, it's kind of amazing how aware you can be of the attention that flows to a resource in the blogosphere.
  </blockquote>

  <blockquote class="speaker_4_text"> 
  <cite class="speaker_4" >Dan:</cite>
      It's amazing, yes.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      On the other hand, it's incredibly fragmentary if there multiple manifestations of that URL. So this question of what is the canonical thing that is the attention attractor, is something I think a lot about, and I'm wondering how that would map into this space. So, we are kind of back to that question, you can have an openURL, I'll call it a query, which can look lots of different ways, the ordering of the parameters could vary, the values of the parameter could vary because the resolver, like you said, could fix things up. So even if can't get the title quite right, it might fix that for you.
      
      You might have varying amounts of detail encoded in the queries, so some resolvers could go all the way down the page, other could only get you down to the article. So it seems you're set up to generate lots of different variance of that query, on the other hand that query is an URL that you want to function as an attention attractor, then you have to canonicalize that somehow. What is the canonicalized version of it?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      [laughing] well, this is the sloppy underbelly of libraries again. To me, I look at this and say, there isn't an easy answer and that's all there is to it. It's sloppy, and you go again back to what, no matter how much work you can do to provide physical mechanisms on the Internet to tie these things together to weave them into a singular fabric, somebody is going to jot it down on paper. And when you jot it down on paper and type it back in, noise gets into the system.
  </blockquote>

  <blockquote class="speaker_3_text"> 
  <cite class="speaker_3" >Jon:</cite>
      In principal, what do you think the canonicalized version could be or should be?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      I think this gets into deep questions of philosophy that I'm not trained to answer. You've been writing recently about surface area... and your surface area of publishing. I couldn't help but think of that when you were talking about expressions, which is the magic trigger to librarians, like me, because we have this model called, FRBR, the Functional Requirements for Bibliographic Records, that talk about the relationship between works of authorships and variations on those such as expressions of a musical work or versions, additions of a printed book and so forth. And expressions is a keyword in that phrase.
      
      So, when you think about an object of some platonic form, the surface area of the expressions of that object is pretty diverse. And the more popular something is, the more thorny shapes and little drop outs you're going to have over that topology. One of which is metadata representations of it that is essentially surrogate the in hand copy which you don't have when you're looking at it.
      
      Sort of by definition, there is loss between representing an object through metadata and the object itself. Particularly when it's hard to say what the object itself really is when we have PDF copies and HTML copies, AAC files and MP3 files and so on, and transcripts of the following.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Apart from the fact that there is, at least according to many people, no apparent business model to support this yet, I can at least imagine a scenario in which the log publishing software thinks in a similar way to, let's say book publishing. Through my experiments with library lookup, I learned more than I ever imagined I would learn about ISBN and that whole system. And as a matter of fact, it does work out pretty well at this point. So, for the versions of the library lookup that go through the OCLC, the service that takes an ISBN, which is one of those belonging to the cluster....
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Right, xISBN.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      ...yes, xISBN, that's a pretty workable scheme, I think. And in principle, we already have in the blogworld, we have this notion of quids, we don't use them very much. It could work without a whole lot of fuss, except it's not a problem that's interesting to many people. We think about what happens in the blogosphere as this throw away stuff. Or at least most people do, I don't, at all. For most people its this transient stuff. We haven't set it up to be a venue for really serious long-term stuff, but why shouldn't it be?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      That's a good question. Certainly places like the Internet archiver are offering their answers to that question. It certainly a new format for knowledge transfer even though it feels like it's been around our whole careers, I know it's been around less than your whole careers, I know it's been around less than your whole career. It was new at the start of mine, basically.
      
      There are a lot of norms to be developed. On the one hand, what you're describing seems to be likely, that a gradient will begin to develop between things that have a more of a permanent nature and things that don't. Systems will be refined and improved to support the things that have more permanence. But on the other hand there's this great phrase that showed up on a Book Arts Press annual mailing a few years ago. Mess is Lore.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      What is it?
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Mess is Lore.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      OK.
  </blockquote>

  <blockquote class="speaker_4_text"> 
  <cite class="speaker_4" >Dan:</cite>
      As opposed to Less is More.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      I like that.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      The noise that comes up in these things is the stuff of legends. Over time, if you look at what libraries and archives do, they end up essentially throwing a lot of things out. Things don't get saved. Floods hit towns and priceless remarkable collections like we had in New Orleans get lost. They get turned into mush and it's tragic.
      
      But this is in some ways simply just what happens over time. To a large extent you really expect and hope that the best stuff gets kept reliably, but on the other hand we know that it doesn't.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      One of Tony's points is he talked about strategic resources. He said, &quot;Look, you're not going to make this investment in everything. But we're in the business of making this investment in scientific discourse because we think it matters and we think it matters for the long term.&quot;.
      
      I guess I would just like to hope that there's a business model for someone in enabling somebody like me who looks at blogging as really quite a professional activity. For me to be able to make a similar investment, it's my intellectual life and I take it very seriously and I constantly refer to things in the past that I have written and just the other day I had to try to go back to something in the <a href="http://byte.com/" >byte.com</a> archive from ten years ago and already that's problematic.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes, sure, sure.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      More and more people, at least I hope it will turn out this way, will be engaged in this activity that originally Dave Wiener called narrating your work. It's a wonderful phrase and a wonderful evocative way of getting at what all this is still becoming. And it isn't that for many people, right? I mean I think blogging for a lot of people is punditry.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      We've sort of created a nation of pundits now, right? Everyone's like, &quot;Oh, I have a blog now. I have a soapbox, I can rant about whatever.&quot; As opposed to, &quot;I have a blog, I can articulate my public agenda in a way that forms this long term record that helps advance my agendas and helps other people understand who I am and interact with me in a serious and professional and productive way.&quot; And when you look at it that way, you can see that yes, I absolutely would pay five or ten bucks a month to have some durability and consistency and reliability to all of this stuff.
  </blockquote>

  <blockquote class="speaker_4_text"> 
  <cite class="speaker_4" >Dan:</cite>
      Yes, absolutely. I don't disagree with you at all. I think we can actually probably learn a lot by looking at the ways we're already trying to address these things. I've recently become a big fan of S3 partly from your discussion of it and hearing from other people.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Yes.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      I'm writing a column now, I've got these few blogs, I've got a lot of code and data I like to keep. I'm very religiously keeping stuff in S3 using Jungle Disc and some scripts and so forth. And that's a relationship between me and Amazon, which doesn't really care about me as an author, or me as a coder. On the other hand, you're not going to ask Amazon to republish your works after you die, if you pass away. That's not the relationship you've entered into. On the other hand, maybe there's an assumption that the Internet Archive will continue to keep some of your stuff alive because that's what their institutional mission is to do.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Right.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      If you go from one of those extremes to the other and bit preservation versus web archiving and these different missions I think you're going to find a lot of these same differentials that we talked about a little earlier between individual responsibility and institutional role.
      
      Certainly for academics the role of the institution in many ways is to promote and somewhat protect the reputation of a researcher or a professor by simply standing behind them and employing them on one hand if they are tenured and whatnot. But also archives exist to take on the papers of important scholars and members of the public sphere and authors, artists and organizations, governments, big companies.
      
      It is the ongoing imperative mission of archives and other libraries to do this work. So, until there is an organization that chooses as it's mission to preserve my bits as an individual, I can't assume that Amazon will or the Internet Archive will because I haven't made that arrangement with them.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Yes.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      I'm not huge you know, I haven't been published like you have and people have been reading in multiple levels of publications every time. Your papers are probably going to be really interesting, I would presume, to maybe the computer history museum or another archive that collects in a similar field someday.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      I'm an outlying data point because I've put a pathologically large amount of stuff onto the net over the last ten or so years. But I really am thinking in terms of anyone, any professional person and the way in which that professional life is going to be publicly represented as a trail of documents and that trail of documents will have been published to the Internet in one form or anther and I'm certain there is a business model here for somebody to help every ordinary person with this problem of long term archiving, persistent reference publication.
      
      If I have any influence at Microsoft, which I probably don't, at product development that would be one thing that I would love to nudge it's online properties in the direction of doing because I think it's something that a lot of people will ultimately want.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Yes, I think it's a great business opportunity. Just to turn your notion of being an outlier on it's head, archives and libraries exist to support outliers, right? Presidential libraries are very unusual. They are only there for presidents.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Yes.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Archives, like the manuscripts and archives unit at Yale exist to collect materials for outliers of society, people who have been prodigious artists or public figures. Now it would make a lot of sense I think to take a good look at that business model and think about cost structures. What would it mean for some random blogger like me to deposit my materials. What would be the arrangement that organization and I would have? What would be the trigger event that would cause them to turn on copies of my stuff.
      
      Or if you enter into an arrangement like that what do you end up doing when you recognize that literally publishing and republishing don't necessarily have to be disconnected? Should there be a permanent <a href="http://wordpress.com/" >wordpress.com</a> or long term <a href="http://typepad.net/" >typepad.net</a> or whatever the popular - <a href="http://blogger.com/" >blogger.com</a>, should there be a long-term <a href="http://blogger.com/" >blogger.com</a> where it's not free, you pay. You pay maybe a lot more than you normally would and the presumption is the extra payment you make is in exchange for a long-term agreement to keep your work alive.
  </blockquote>

 <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Absolutely. I'd pay for that in a heartbeat if I were convinced that the promise can be kept which of course is a really tricky thing.
  </blockquote>

  <blockquote class="speaker_4_text"> 
  <cite class="speaker_4" >Dan:</cite>
      Well the great thing is that a lot of people listen to you and I hope some of these people get that idea and we see some of these services soon. But I'd still want to really seriously consider the agreement that you enter into with the organizations.
  </blockquote>
  
  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Yes.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
 You want to look at their board of directors and their financial structure. You'd really want to take that arrangement very seriously as an individual, probably much more so. You'd want to think about it more in terms of the amount of consideration you give writing your will.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Yes, because we really are talking about the long run here. The only real security in this model is that if it is a valid business model that works then it will be in someone's interest to continue to hold up some version of that model over time. If it makes sense as a business then someone will want to operate that business at that point and it can change hands. If it doesn't make sense as a business then it's not going to fly.
      
      This was like a lot of fun.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      It sure is.
  </blockquote>

  <blockquote class="speaker_3_text"> 
  <cite class="speaker_3" >Jon:</cite>
I was thinking it would be really interesting to circle back and talk to you after you've been at the Library of Congress for a while, unless of course what you do there winds up being secret. I don't know if it would.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
I think some of what they do is probably, but I really don't know what projects I'm going to be working on.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Thanks so much.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Thank you. It's a real pleasure.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
I will be following your adventures. I assume that you will, to the extent that you can, be blogging about your life at the Library of Congress.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      As soon as I get there and learn my way around, I hope to be, yes.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Excellent.
  </blockquote>

  <blockquote class="speaker_4_text">
  <cite class="speaker_4" >Dan:</cite>
      Thank you. All right Jon.
  </blockquote>

  <blockquote class="speaker_3_text">
  <cite class="speaker_3" >Jon:</cite>
      Take care.
  </blockquote>

</div> 
