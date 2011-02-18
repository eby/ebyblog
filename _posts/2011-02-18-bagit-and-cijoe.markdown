--- 
layout: post
title: Bagit Validation and CIJoe
categories: code4lib
---

I've started playing around with [bagit](https://confluence.ucop.edu/display/Curation/BagIt) and some of the other [curation microservices](https://confluence.ucop.edu/display/Curation/Home). One of the features involved is manifest files w/ checksums of all the data files in the bag. So far I'm still just getting the hang of it but decided to try [cbeer's bagit gem](https://github.com/cbeer/bagit) and try hooking the validate function to [cijoe](https://github.com/defunkt/cijoe) integration server. With the bag in git repository it was easy to have cijoe run a simple script that returned zero when validated, or one with output if there was a problem. cijoe can use git hooks to notify via various methods (example one for email is given in repo).

While not robust it only took a minute to get the output displayed:

![bagit and cijoe](http://farm6.static.flickr.com/5253/5455986619_3296f6881b.jpg)
[larger version](http://www.flickr.com/photos/ebyryan/5455986619/sizes/l/)

A few thoughts:

* need to tweak cijoe to work on local repository instead of requiring an origin
* keeping the validation script in the repository helps. should probably validate/manifest it as well

Overall a lot easier than I thought it would be and serves as a simple interface for seeing current status for those who like a webpage. cijoe also has jsonp and a simple http status api that allows other tools to easily look at build status so seems like it could be an easy tool to run all your tests in one place and let various things ping it.