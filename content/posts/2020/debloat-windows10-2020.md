---
title: "Debloat Windows in 2022"

date: 2020-06-11T16:04:48-05:00
url: /debloat-windows-10-2020/
image: images/2022-thumbs/cleanup-windows-2022.jpg
categories:
  - Windows
tags:
  - Microsoft Store
featured: true
---
This goes over debloating and slimming down Windows 10 so you get maximum performance from your PC. 
<!--more-->I made a guide going over the debloat process two years ago [https://christitus.com/debloat-windows-10/](https://christitus.com/debloat-windows-10/) - The guide has evolved and the github project I was using has also improved.

## April 2022 Update

- Added new options to get Windows 10/7 Options in Windows 11
- Service optimizations to reduce process count
- Added more tweak settings and misc. fixes

New shorter command! (_old command still works though..._)
```
iwr -useb https://git.io/JJ8R4 | iex
```

## July 2021 Update

If you are coming here from the YouTube video I have taken all the scripts below and a system admin script I used a lot in the past to make a streamlined debloat script. This script will optimize Windows and can be run multiple times if you have an update ruin all the optimizations. I have also made it very easy to launch. Here is the source files: <https://github.com/ChrisTitusTech/win10script>

If you want to just run this on any system, you can easily copy and paste this into a Admin Powershell prompt and watch it do everything for you. It does have two prompts based on user feedback. Let me know what you think below! 

*December 2020 Feature: GUI added - Select what you want!*
*January 2021 Feature: 10 Bug Fixes and Network Optimizations added*
*July 2021 Updates: 30+ Bug Fixes and Undo Options added*

```
iex ((New-Object System.Net.WebClient).DownloadString('https://git.io/JJ8R4'))
```

### What this script can do

- Installs any program listed that you click on using WinGet
- Removed Telemetry
- Disables Cortana
- Deletes various schedules tasks that rebloat the system
- Fixes problems that other scripts causes (lock screen and personalization options restricted)

Based on User feedback Microsoft Store and Windows Defender is no longer touched. 

### Toolbox Walkthrough Video

[![win10toolbox](https://img.youtube.com/vi/V27McA7ch6w/0.jpg)](https://www.youtube.com/watch?v=V27McA7ch6w)  
_Note: YouTube Video - Hold Ctrl + Left Click to open in new window_

## User Requested Restore Scripts

```
iex ((New-Object System.Net.WebClient).DownloadString('https://git.io/JTbKD'))
```

This restore script pops up a GUI that lets you restore what you want to FACTORY DEFAULTS! 

Current Lineup:
- Cortana
- Tray Icons
- Action Center

## Old Methods from Prior Videos that I no longer use
The project I use has been developed for many years now and is extremely good. Here is the source github project I use:  
[https://github.com/Sycnex/Windows10Debloater](https://github.com/Sycnex/Windows10Debloater)

This is a new project that was brought to my attention, but has quickly made a name for itself. It works very well and is typically more up to date than the above project.  
[https://github.com/farag2/Windows-10-Setup-Script](https://github.com/farag2/Windows-10-Setup-Script)

## Optimal Way to Use this Tool

I recommend running this tool under the following conditions:
  - Before User Profile is Created
  - Empty Desktop and Downloads (Past versions has deleted files from Desktop and Downloads)
  - After installing New Feature Updates
  
Recommended Options:
  - Disable Cortana
  - Uninstall OneDrive
  - Run Essential Tweaks
  
I generally always enable Dark Mode and Install 3.5 .NET but that is entirely my personal preference. 
  
