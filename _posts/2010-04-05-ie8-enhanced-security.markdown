--- 
layout: post
title: IE8 Upgrade and Enhanced Security Stuck For Some Profiles
---

Had an issue with IE upgrades in the recent past where after the upgrade multiple pre-existing profiles would  state they were in "Enhanced Security Mode" despite that mode being disabled. New profiles will work fine and Administrator usually does.

From what I've been able to track down, MS hasn't figured out the exact circumstances that cause it. Fresh installs w/ upgrades before anyone logs in seem to work fine here as well. Searches brought up multiple hacks to fix it. One is to make a login script that modifies the registry like so for every user:

    [HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Internet Settings]
    "IEHardenIENoWarn"=dword:00000000

    [HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Internet Settings\ZoneMap]
    "IEHarden"=dword:00000000

The best solution I found though was to use GPO and force a setting for the Internet Zone. Forcing it to Medium or whatever level appears to get pass the enhanced security issues and things work like normal.

Under either User or Computer depending on how you have GPO setup

    Administrative Templates>Windows Components>Internet Explorer>Internet Control Panel>Security Page>Internet Zone

Not ideal but I've it is the best I've found