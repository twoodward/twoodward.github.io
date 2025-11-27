---
layout: post
description: "Learn how to protect your radio station's Barix audio codecs from hijacking attacks with VPN tunneling, firewall configuration, and IoT security best practices."
title: "How to Protect Barix Audio Codecs from Radio Broadcast Hijacking"
date: 2025-11-03 06:00:00 -0500
image: 'images/barix-hijacking.jpg'
video_embed: https://www.youtube.com/embed/G8av5rHRYsI?si=JE3Rx9-xw57viMAB
tags: [Episodes]
tags_color: '#008800'
featured: false
toc: true
---

Over 600 [Barix Instreamer and Exstreamer](https://www.aareff.com/en/barix-instreamer-and-exstreamer-audio-codec-set/) devices are sitting exposed on the public internet right now, discoverable through [Shodan](https://www.ituonline.com/how-to/how-to-discover-iot-devices-with-shodan/) searches by anyone with basic technical knowledge. If your radio station uses Barix equipment for your [studio-to-transmitter link](https://www.youtube.com/watch?v=Az5W_1dnJMc), your audio airchain could be completely compromised without proper security measures.

The Labor Day weekend 2025 attacks on stations like KPOG in Des Moines and KRLL in Missouri weren't isolated incidents. They were wake-up calls for an industry that's collectively behind on cybersecurity.

## The Labor Day Weekend Attacks

During Labor Day weekend 2025, hackers hijacked multiple radio stations through vulnerable Barix audio codecs. KPOG, an LPFM station in Iowa, suddenly broadcast explicit content and fake [Emergency Alert System](https://en.wikipedia.org/wiki/Emergency_Alert_System) messages. KRLL in Missouri suffered the same fate.

The common thread? Both stations used [Barix equipment](https://www.barix.com/) to send audio from their studios to their transmitter sites. The devices were directly accessible from the internet, making them easy targets for exploitation.

## Why Barix Devices Are Vulnerable

[Johannes Rietschel](https://www.radioworld.com/news-and-business/news-makers/barix-founder-and-cto-bangs-security-drum), founder and CTO of Barix, has been sounding the alarm on this issue for years. The Switzerland-based company has sold approximately 1.4 million audio over IP devices worldwide since 2001. Tens of thousands of second-generation Instreamer encoding devices and Exstreamer decoding devices, released in 2003, are still in use at stations today.

The problem isn't the devices themselves. Barix has never marketed these as plug-and-play, all-in-one appliances. The Exstreamers are, at their core, generic [IP audio decoders](https://en.wikipedia.org/wiki/Audio_codec) that require proper network security configuration.

## How the Attacks Work

Hackers use automated search engines like Shodan to locate exposed devices on the public internet. All they need is an IP address and operating port of a device. Once located, poorly secured Barix codecs become an easy entry point into a station's audio airchain.

If an attacker gains access to a station's Barix equipment, they can inject any audio content they want. This includes explicit material, fake emergency alerts, or even execute a complete [distributed denial of service attack](https://en.wikipedia.org/wiki/Denial-of-service_attack) that renders the entire network unusable.

## The Core Security Problem

Twenty years ago, there wasn't much talk about IT security in broadcasting. Radio stations praised Barix equipment for its ease of setup and cost-effectiveness. The reliability of these devices became both a blessing and a curse, as stations installed them and forgot about security entirely.

In 2015, several high-profile breaches of Barix devices led to an [FCC investigation](https://www.fcc.gov/). Yet the problem persists today. Budget cuts, scant technical staff, and the "if it ain't broke, don't fix it" mentality have left hundreds of stations vulnerable to attack.

## VPN Tunneling: The Gold Standard

Rietschel's recommendation is clear and absolute. Barix devices should never be fully exposed to the internet. The gold standard for security is implementing a [VPN tunnel](https://en.wikipedia.org/wiki/Virtual_private_network) between your studio and transmitter site.

A VPN creates an encrypted connection that makes your Barix equipment invisible to the outside world. Even if your studio and transmitter are on two separate LANs, a properly configured VPN keeps everything secure behind firewalls.

## Barix Reflector Service

For stations without in-house IT support, Barix offers the Reflector Service, launched with Streamguys over 15 years ago. This service matches authenticated Barix decoders and encoders and forwards the stream between them. Both devices stay protected behind firewalls and remain invisible to the public internet.

The Reflector Service costs a modest monthly fee but was designed specifically for this security situation. It's a turnkey solution for stations that lack the technical resources to implement VPN tunneling themselves.

## Stream Pull Configuration

Another alternative is Barix's "stream pull" method, known as BRTP. This configuration allows the Exstreamer decoder to sit on a dynamic IP address behind a firewall and pull a stream from an Instreamer in the studio.

The studio still needs a public IP address, but only one specific port needs to be forwarded. A properly configured [firewall](https://en.wikipedia.org/wiki/Firewall_(computing)) can limit access so the device isn't detectable on sites like Shodan.

## Port Forwarding Risks

Many stations configure their Barix equipment with simple port forwarding, thinking this provides adequate connectivity. It doesn't. Port forwarding exposes your devices directly to the internet, making them discoverable and vulnerable.

Rietschel compared this approach to making your home printer available to the world, then being surprised when hackers drain all the ink. Any [IoT device](https://en.wikipedia.org/wiki/Internet_of_things) with an open port accessible from the outside internet is vulnerable, regardless of manufacturer.

## Industry Expert Insights

Fletcher Pride from Family First Radio Network, Shane Toven from Frandsen Media, and other industry experts emphasize that securing broadcast equipment is no longer optional. The next generation of broadcast engineers often deals with IT security daily and understands these concepts intuitively.

Smaller stations should start by talking with whoever originally set up their Barix equipment. If the system was successfully paired in the first place, the station has the technical capacity to secure the devices properly.

## Next-Generation Barix Devices

Barix has offered a next generation of audio devices for about seven years, equipped with recent security features. However, even with newer models, Rietschel's core warning remains absolute. Never put any IoT device on the public internet without proper security measures.

The reality is that legacy equipment will remain in service for years to come. Upgrading to newer devices is helpful, but not a substitute for proper network security practices like VPN tunneling and firewall configuration.

## Actionable Steps for Station Engineers

First, check if your Barix equipment is exposed on Shodan. Search for your station's IP addresses and see what shows up. If your devices appear in search results, they're vulnerable.

Second, implement VPN tunneling between your studio and transmitter site if technically feasible. This is the most secure approach and should be your primary goal.

Third, if VPN implementation isn't immediately possible, consider the Barix Reflector Service or stream pull configuration as interim solutions. These provide significantly better security than direct internet exposure.

## The Bigger Picture

The Barix hijacking incidents are part of a larger trend in broadcast cybersecurity. As the radio industry pushes more critical systems into the cloud and relies on internet connectivity for essential functions, the attack surface grows exponentially.

Securing your audio codecs is just one piece of the puzzle. Stations need comprehensive cybersecurity strategies that protect every internet-connected device, from [STL equipment](/tags/stl/) to automation systems to emergency alert decoders.

## Technical Fluency Matters

For years, the radio industry has preached being nimble in areas like podcasting, marketing, and video. Technical knowledge, particularly in cybersecurity, should be at the top of that list.

Maybe it's a younger staffer who's more fluent in this area. Maybe it's bringing in an outside IT consultant. Either way, your station deserves the same level of network security you'd expect at home or in any modern office environment.

Radio stations are community resources and trusted sources of information, especially during emergencies. Allowing your broadcast infrastructure to remain vulnerable doesn't just risk embarrassing on-air incidents. It potentially compromises public safety.