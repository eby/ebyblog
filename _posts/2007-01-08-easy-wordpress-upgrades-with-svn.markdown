--- 
wordpress_id: 433
layout: post
title: Easy Wordpress Upgrades with SVN
wordpress_url: http://blog.ryaneby.com/archives/easy-wordpress-upgrades-with-svn/
---
I came across these hints in some comments on blogs but don't have them bookmarked so credit to other people. This probably isn't a supported install method either, so use at your own risk. I've found it easier than the normal process though.

You may be aware but Wordpress uses Subversion and Trac for their development. This means you can check out the source which means you can also easily upgrade your source. There's two ways you can do this:

<h4>1. Check out the current branch.</h4>

The current branch appears to have the upgrades. What you do is checkout the branch with the revision of the last tagged release. When an update occurs then you can checkout that revision. Or you can just update to the branch and you will get the beta's and release candidates for releases of the branch. Probably not as stable but I didn't have any problems.

Note: I did have a problem with the branch as it pulled in the akismet plugin from svn that didn't seem to work. You may want to remove it from svn on your local install or install it manually.

<h4>2. Check out the tag.</h4>

Another option is to checkout the latest tag. When an update occurs then you do a svn switch to the new tag.

<code>svn co http://svn.automattic.com/wordpress/tags/2.0.5/</code>

<code>svn switch http://svn.automattic.com/wordpress/tags/2.0.6/</code>

<h4>Some notes</h4>

<ul>
<li>Remember to run the wp-admin/upgrade.php<li>
<li>Your config file won't be under SVN so won't be overwritten</li>
<li>If you modified templates you may want to make sure they are in their own folder and not under svn.</li>
<li>Trac - <a href="http://trac.wordpress.org/">http://trac.wordpress.org/</a></li>
<li>SVN - <a href="http://svn.automattic.com/wordpress/">http://svn.automattic.com/wordpress/</a></li>
</ul>

So far I've been doing this for the 2.0 line and haven't had a problem. Made the process much easier then copying files and hoping I remembered everything.
