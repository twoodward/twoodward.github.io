---
layout: post
description: Windows 10 support officially ends on October 14, 2025. For radio and TV stations, that is not just an IT problem. It is a potential on-air disaster waiting to happen.
title: "Microsoft Is Killing Windows 10, and That’s a Huge Problem for Broadcasters!"
date: 2025-10-07 08:00:00 -0500
image: 'images/Win10_Deadline.jpg'
tags: [Engineering]
tags_color: '#444444'
featured: false
toc: true
---

Microsoft is finally shutting down support for Windows 10. On **October 14, 2025**, the company will stop releasing updates, patches, and security fixes for one of the most widely used operating systems in the world.  

For most people, that means an annoying popup and maybe a weekend project. For broadcasters, it could mean silence on the air.

## When the updates stop, the problems start

Inside almost every radio or television facility, there is at least one computer quietly running Windows 10. Maybe it is an audio logger in a back closet, a playout server feeding automation, or a PC controlling remote transmitters. These systems are the backbone of modern broadcasting. They are stable, they work, and most engineers avoid touching them for that exact reason.  

The problem is that stability comes at a cost. Once Microsoft stops sending updates, those machines stop being secure. Every known flaw becomes permanent. Hackers and ransomware groups watch these end-of-life dates carefully, waiting for when systems are left unpatched and vulnerable.  

In 2017, the **[WannaCry ransomware outbreak](https://www.bleepingcomputer.com/news/security/the-wannacry-ransomware-outbreak/)** spread through unpatched Windows systems around the world. Hospitals, shipping companies, and government offices were hit within hours. Microsoft had already issued a patch that could have stopped it. Many organizations never installed it.  

And in 2021, **[Sinclair Broadcast Group](https://www.axios.com/2021/10/18/sinclair-broadcast-group-cyberattack)** faced a cyberattack that disrupted dozens of local TV stations. Automation systems failed, traffic scheduling went offline, and some stations were left scrambling to get back on air. The company never released full technical details, but cybersecurity analysts pointed to outdated and unpatched Windows servers as one possible weak point.  

When updates stop, attackers move in. That is the reality Microsoft is leaving behind for anyone who does not upgrade.

## Outdated does not mean harmless

Walk into almost any transmitter building or master control room and you will find a tower PC running something critical on Windows 10. It might be managing your Emergency Alert System. It might be feeding an STL encoder. It might even be running automation that has not been rebooted in years.  

These are the boxes people are afraid to touch. They are often connected to internal networks that also handle automation, logging, and sometimes even corporate file shares. When one of them gets infected, the damage spreads fast.  

Antivirus software can help, but it cannot make up for missing operating system patches. Once Windows 10 stops getting security updates, even the best antivirus will be a stopgap. A single exploit can bypass protections, encrypt local drives, and lock up every shared resource it can reach.  

For broadcasters, that means playlists stop, routers freeze, and dead air follows. A ransomware attack is not just an IT inconvenience. It is an operational crisis.

## Microsoft will still take your money

Microsoft knows not everyone can upgrade. Some stations rely on legacy software that will not run on Windows 11. Others use hardware with older CPUs that do not meet the strict Windows 11 requirements like **TPM 2.0**, **Secure Boot**, and **UEFI firmware**.  

For those cases, Microsoft offers a temporary escape route called **[Extended Security Updates](https://learn.microsoft.com/en-us/windows/whats-new/extended-security-updates-windows-10)**, or ESU. It allows organizations to keep receiving patches for a few more years after official support ends.  

The problem is cost. The ESU program is designed for hospitals, governments, and large enterprises, not for small or medium broadcast stations. The price increases each year, eventually exceeding the cost of replacing or upgrading the system entirely. Paying for ESU is like paying rent on a building that is already condemned.

## The free fix that is still available

There is a better option. If your system meets the requirements, you can still **upgrade to Windows 11 for free**.  

Microsoft’s activation servers continue to accept valid Windows 10 licenses. If your hardware has a compatible TPM chip and Secure Boot enabled, the upgrade is straightforward. Download the **[Windows 11 Installation Assistant](https://www.microsoft.com/en-us/software-download/windows11)**, back up your data, and plan for a few hours of downtime.  

For engineers managing multiple systems, the process can be automated with tools like Windows Deployment Services or Microsoft Deployment Toolkit. With a little preparation, an entire facility can be updated overnight.  

Windows 11 is not perfect, but it is supported, secure, and ready for modern hardware. Most importantly, it will continue to receive critical patches long after Windows 10 has gone dark.

## When “if it works, don’t touch it” becomes dangerous

The broadcast industry has always been cautious about software updates. That caution made sense when stability was the top priority. The problem is that a stable but unpatched system is a ticking time bomb.  

Imagine a playout server that feeds your 24-hour programming suddenly locking up because of ransomware. Now imagine the same malware spreading to your EAS encoder, your traffic scheduler, or the VPN connection you use to reach the transmitter site.  

The result is the same every time. You go silent. Listeners leave. Viewers change channels. Engineers drive hours to fix something that could have been avoided with an upgrade.  

This is not hypothetical. Similar attacks have already taken major broadcast groups off the air. It can happen again, and next time it might target smaller stations that lack large IT budgets or redundant systems.

## Plan before the deadline

October 14 is not just a random date on a calendar. It is the line between supported and abandoned.  

Now is the time to make a list of every Windows 10 system in your plant. Check which ones can be upgraded, which ones cannot, and which ones need to be replaced entirely. Even a modest desktop with a modern CPU can handle Windows 11. If you are running older hardware, consider migrating its function to a virtual machine or dedicated appliance.  

For systems that must stay on Windows 10 temporarily, isolate them from the rest of your network. Turn off unnecessary shares, disable external internet access, and make sure backups are current. These steps will not stop an attack forever, but they will limit the damage.  

Broadcast chains are only as strong as their weakest link. In 2025, that weakest link might be a forgotten Windows 10 PC in the corner.

## Do not wait for silence

Broadcasters spend endless time planning for power failures, transmitter faults, and fiber cuts. Backup transmitters, redundant STL paths, and generator failovers are standard. But when a ransomware attack hits the system feeding your air chain, all that redundancy collapses.  

This is not about new features or fancy operating systems. It is about keeping the signal alive.  

If you wait until Windows 10 support ends, you are already behind. Upgrade now, replace what you can, and secure what you cannot. The silence you save might be your own.