--- 
layout: post
title: Forcing Download with nginx
categories: code4lib
date: 2011-04-06 18:00:00
---

Prompting a browser to download rather than open something is rather common. You can do so from your favorite web programming language by adding the Content-Disposition attachment header when sending the data back.

This can come in handy if you want to use the same file for both web serving and download. Say a MP4 movie file. It makes it a little easier than the right-click save-as method.

If you want to remove the overhead of serving a file through a script you can also accomplish this straight in [nginx](http://wiki.nginx.org/). In the example below the file can be served both ways.

Served normally: http://example.org/mymovie.mp4

Served as attachment: http://example.org/mymovie.mp4?name=mymovie.mp4

This would go inside the location declaration:

{% highlight nginx %}
  if ($args){
    add_header X-Content-Type-Options nosniff;
    add_header Content-Type "application/octet-stream";
    add_header Content-Disposition 'attachment; filename="$arg_name"';
  }
{% endhighlight %}

This also gives you the option of having the downloaded file be named differently. So if you have directory structure like /2011/mysong.mp3 you could have it save as 2011-mysong.mp3.

This also lets you take advantage of other nginx features like [X-accel](http://wiki.nginx.org/X-accel) when serving or streaming the files.