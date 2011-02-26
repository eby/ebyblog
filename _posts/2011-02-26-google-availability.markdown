--- 
layout: post
title: Availability in Globally Distributed Storage Systems
categories: code4lib
date: 2011-02-26 13:00:00
---

Google just released a research paper entitled [Availability in Globally Distributed Storage Systems](http://research.google.com/pubs/pub36737.html). It is available for download in PDF format (14 pages). From the abstract:

> We characterize the availability properties of cloud storage systems based on an extensive one year study of Google's main storage infrastructure and present statistical models that enable further insight into the impact of multiple design choices, such as data placement and replication strategies. With these models we compare data availability under a variety of system parameters given the real patterns of failures observed in our fleet.

It is worth taking a quick browse of. The paper focuses on data availability (online versus data backup/integrity) and includes things like planned downtime. Metrics are given to assist in system design. Some highlights:

* GFS waits around 15 minutes before trying recovery process as that is more than the average time a node might return itself to normal operation (reboot, etc)
* Many events are rack and multi-rack level (network, rolling reboots, etc)
* Failures tend to happen in bursts
* Important to take the above two into account when planning replication schemes
* Reboot time is important
* Storing data across data centers reduces data unavailability by many orders of magnitude compared to having the same number of replicas in a single data center