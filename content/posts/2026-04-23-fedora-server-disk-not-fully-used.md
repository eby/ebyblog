--- 
title: Fedora Server Doesn't Use the Entire Disk on Fresh Install
date: 2026-04-24 11:00:00
---

Recently did a fresh install of Fedora Server 43 and noticed it only used about 15GB of disk space with the default automatic partitioning.

Searching found that this is by design on the server version as it presumes you will add workload specific partitions.

> It always leaves a lot of free space on the assumption that you will need to create work load specific partitions.
>
> Normally this is the right choice.
> 
> [Fedora 43 fresh setup did not use entire drive](https://discussion.fedoraproject.org/t/fedora-43-fresh-setup-did-not-use-entire-drive/188451)

Mine defaulted to LVM so it was a quick 

`sudo lvextend --resizefs --extents +100%FREE /dev/mapper/fedora_fedora--public-root`

Reference: [Extend a Logical Volume on Linux](https://www.andreaslongo.com/blog/unix-lvm-extend-logical-volume/)
