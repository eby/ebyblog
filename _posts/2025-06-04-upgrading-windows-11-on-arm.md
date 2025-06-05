---
layout: post
title: Upgrading Windows 11 ARM from 22h2 or 23h2
date: 2025-06-04 15:31 -0400
---

I run Windows 11 on ARM in Parallels on a Mac Studio for testing.

Windows Update would say up to date but needed to move to the next version of Windows (I was on 22h2 from initial Parallels download). I wasn't offered the option to upgrade to the latest versions.

Solution from various sources:

### 22h2 -> 23h2

You can use an entitlement to enable the update the quickest.

Download: [Enablement Package](https://catalog.sf.dl.delivery.mp.microsoft.com/filestreamingservice/files/c29dd4ea-7f6a-4636-a991-29ba8ae70658/public/windows11.0-kb5027397-arm64_bacb74fba9077a5b7ae2f74a3ebb0b506f9708f3.msu)

[Source](https://www.thurrott.com/windows/windows-11/294170/still-stuck-on-windows-11-version-22h2-you-can-upgrade-to-23h2)

### 23h2 -> 24h2

Create a new registry key (folder) called `Windowsupdate` at:

`Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows`


Then create 3 values within

`Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\Windowsupdate`:

| Name | Type | Value |
| ---- | ---- | ----- |
| ProductVersion | String | Windows 11 |
| TargetReleaseVersionInfo | String | 24H2 |
| TargetReleaseVersion | DWORD | 1 |

Once you check for updates a 24h2 download will start and install.

[Source](https://forum.parallels.com/threads/update-windows-to-24h2-on-arm.364414/)
