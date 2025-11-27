---
layout: post
title: Uptime Kuma! The Open-Source Monitoring Tool Radio Engineers Didn’t Know They Needed
date: 2025-09-22 08:00:00 -0500
image: 'images/uptime-kuma.jpg'
tags: [Tools]
tags_color: '#009999'
featured: false
toc: true
---

Radio stations spend serious money to make sure they never go dark. Dead air isn’t just awkward, it’s expensive. For decades the solution has been purpose-built monitoring hardware like the [Burk ARC Plus](https://burk.com/) or [DPS T/Mon](https://www.dpstele.com/). They work, but they come with enterprise price tags that smaller stations can’t always justify.  

That’s why a surprising new favorite has emerged among engineers: **[Uptime Kuma](https://github.com/louislam/uptime-kuma)**. It’s free, it’s open source, and it’s built with the kind of modern design you’d expect from a Silicon Valley SaaS, not a broadcast gear rack. Instead of a $15,000 controller, you can spin it up on a Raspberry Pi or a small VM and get instant oversight of your most critical systems.  

## What makes it so useful in radio?  

On the surface, Kuma is a general uptime monitor — the kind of tool IT admins use to keep websites online. But broadcast has quietly become an IT-first business. Your airchain is full of IP links, web consoles, and streaming endpoints, and Kuma thrives in that world.  

It can ping routers, check TCP ports, or load web interfaces from devices like [Barix](https://www.barix.com/) and [Tieline](https://tieline.com/) STL units. If something stops responding, Kuma notices before your listeners do. The same goes for automation systems like [RCS Zetta](https://www.rcsworks.com/products/zetta/), [WideOrbit](https://www.wideorbit.com/), and [ENCO DAD](https://www.enco.com/products/dad-radio-automation). Their databases and APIs can be monitored just as easily as a website.  

## Streams don’t go down quietly  

If your station runs [Icecast](https://icecast.org/) or [SHOUTcast](https://www.shoutcast.com/), Kuma can check stream status pages, track listener counts, and confirm CDN endpoints on [Cloudflare](https://www.cloudflare.com/) or [AWS CloudFront](https://aws.amazon.com/cloudfront/).  

One of the sleeper features is its **public status page**. Instead of replying to angry tweets when the stream drops, you can point listeners to **status.yourstation.com**, where they’ll see live updates pulled straight from Kuma. It’s the kind of transparency usually reserved for big tech companies, and it costs nothing.  

## The fine print  

Kuma isn’t magic. It can’t measure audio quality or detect silence, and it doesn’t support [SNMP](https://en.wikipedia.org/wiki/Simple_Network_Management_Protocol). That means no transmitter forward power readouts or UPS battery runtime graphs. If you need deep telemetry, you’ll still want something like [Zabbix](https://www.zabbix.com/) running alongside it.  

But for daily “is it up or down?” monitoring, Kuma nails it. And it does it with more than [90 notification options](https://uptime.kuma.pet/) built in, from email and SMS to [Slack](https://slack.com/), [Teams](https://www.microsoft.com/en-us/microsoft-teams/group-chat-software), [Discord](https://discord.com/), or even automated [Twilio](https://www.twilio.com/voice) calls.  

## The big picture  

Broadcast engineering is increasingly about managing networks, not just transmitters. Uptime Kuma feels like the right tool for that moment. It doesn’t pretend to be a compliance logger or a replacement for high-end control systems. Instead, it delivers the essentials with a clean, modern interface and a price that makes even the smallest station competitive: free.  

The result is simple but powerful. Uptime Kuma can tell you if your stream is online, if your transmitter is reachable, and if your automation system is alive. For most stations, that’s 80 percent of the fight — and it costs less than lunch.  
