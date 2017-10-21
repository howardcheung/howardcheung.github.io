---
layout: post
title:  "Dual boot with Windows and Linux"
date:   2017-10-21 15:00:00 +0800
categories: ["Computer"]
comments: true
---

I tried to use [lubuntu](http://lubuntu.net/) in the past to see if I could get used to Linux. Unfortunately, it didn't work. The laptop I used to put lubuntu on was too old. I also got a lot of problems when I tried to use my webcam. Even the Wi-Fi took a long time to set up. I was quite frustrated.

It was quite a few years since then. Recently I got a laptop with much more hard-drive space. This means that I would have space for two operating systems, right? So I decided to give it a try again.

Instead of using lubuntu, this time I decide to try [Linux Mint](https://linuxmint.com/).

![](../../../../raw_img/Computer/LinuxDualBoot.png "My Linux Mint installation")

After the installation, I found the operating system to be quite easy to use. No additional effort was needed to set up the Wi-Fi. The programming languages that I often used were pre-installed unlike Windows. Most of the applications like LibreOffice, Firefox, Thunderbird, etc. were pre-installed as well. The whereabouts of the applications were also similar to that of Windows and were easy to find.

However, the painful part was the installation of the operating system itself. Because I was preserving my Windows, I could not wipe out the hard-drive. Since my last operating system installation was conducted before the days of [UEFI](https://en.wikipedia.org/wiki/Unified_Extensible_Firmware_Interface) and Secure Boot, I did not know that these things were used in the laptop and required special setting before I could configure my computer to dual-boot with Linux and Windows. It took me several hours to figure out how to run it properly. At the end, I need to use [Boot-Repair](https://help.ubuntu.com/community/Boot-Repair) to fix the issue.

The other problem is about my USB-C-to-ethernet converter. While it could be identified by Linux, Linux failed to have an appropriate driver for it. I needed to keep searching the web for instructions before I found the solution [here](https://chentiangemalc.wordpress.com/2012/10/22/case-of-the-broken-linux-driver-lenovo-usb-2-0-ethernet-10100-dongle/). It took me around 1 to 2 hours to get my ethernet working.

There is still a long way to go before I am familiar with the system. Hope I won't give up this time.
