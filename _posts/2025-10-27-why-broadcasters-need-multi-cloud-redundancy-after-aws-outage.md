---
layout: post
title: Why Broadcasters Need Multi-Cloud Redundancy After AWS Outage
description: "When AWS collapsed last Monday morning, taking Snapchat, Roblox, and half the internet with it, most people saw an inconvenience. As a broadcast network engineer, I saw a nightmare scenario—one that's about to get worse as the industry pushes critical systems, including emergency alerts, into the cloud."
date: 2025-10-27 08:00:00 -0500
tags: [Episodes]
image: /images/aws-outage-broadcast-infrastructure.jpg
video_embed: https://www.youtube.com/embed/VKb2BWaMTV0?si=M53zlDXRLn0cfk0C
tags_color: '#008800'
featured: false
toc: true
---

When [AWS collapsed last Monday morning](https://www.reuters.com/business/retail-consumer/amazons-cloud-unit-reports-outage-several-websites-down-2025-10-20/), taking Snapchat, Roblox, and half the internet with it, most people saw an inconvenience. As a broadcast network engineer, I saw a nightmare scenario—one that's about to get worse as the industry pushes critical systems, including emergency alerts, into the cloud.

Here's the problem: imagine your home internet goes out. Annoying, right? Now imagine you're a business that depends on that connection, but you smartly have Spectrum as your primary and Lumen as backup. When Spectrum fails, Lumen takes over. You stay online. That's basic redundancy, and most critical businesses figured this out years ago.

Radio stations? Many are putting their entire automation systems on AWS with no backup. When Monday's [DNS failures](https://www.youtube.com/watch?v=KFvhpt8FN18) hit, any station running solely on AWS would have faced dead air, no commercials, no programming, and listeners tuning out in droves. Your most valuable advertising daypart—morning drive—gone. Revenue? Also gone.

## The All-Your-Eggs Problem

I've been working in broadcast engineering since 2018, radio since 2014, and now as a broadcast network engineer. I've seen enough infrastructure failures to know that single points of failure will eventually bite you. [Dave Plummer](https://www.youtube.com/watch?v=KFvhpt8FN18), a retired Microsoft systems engineer who analyzed Monday's outage, explained that DNS failures create a cascading disaster he called "a denial of service snowball." Services don't fail gracefully—they thrash, retry exponentially, and make everything worse. 

While cloud-dependent systems were melting down Monday, broadcast stations with proper infrastructure kept running. We stayed on the air. Because we understood something fundamental that apparently needs repeating: single points of failure are unacceptable when your business depends on staying operational.

But here's where it gets concerning. The broadcast industry is moving critical infrastructure to single cloud providers. I'm seeing automation on AWS. Traffic systems on AWS. Studio-to-transmitter links over single internet connections. It's the equivalent of that business with only Spectrum internet and no backup—when it fails, everything stops.

The solution we need is exactly what you'd tell any critical business: **multi-cloud redundancy**. Run primary automation on AWS, backup on Azure. When AWS goes down (and as Monday proved, even the biggest providers *do* go down), Azure takes over automatically. Programming continues. Ads keep playing. Revenue stays protected. It's the Spectrum-plus-Lumen model applied to cloud infrastructure.

Alternatively, keep automation on-premise with cloud only for disaster recovery. That way, internet outages don't affect your daily operations at all. The cloud is there if your building burns down, but Monday's DNS failures? Not your problem.

## The EAS Cloud Push

Here's where this gets genuinely dangerous, and it's something I feel strongly about. The [FCC has been exploring](https://www.tvtechnology.com/news/nab-urges-fcc-to-allow-software-based-eas) moving the Emergency Alert System to cloud-based platforms. The NAB has been pushing for software-based EAS. Some alerts already arrive via [internet-based CAP/IPAWS](https://www.fema.gov/emergency-managers/practitioners/integrated-public-alert-warning-system) systems.

Traditional EAS works through dedicated on-premise hardware monitoring RF sources. It operates completely independently of the internet. When severe weather hits and I need to relay a tornado warning *right now*, that hardware works whether AWS is up or down. It's been reliable for decades precisely because it doesn't depend on cloud providers, DNS resolution, or internet connectivity.

Now imagine that system in the cloud. Monday's AWS outage happens. Your cloud-hosted EAS is unreachable because DNS is failing. There's an actual tornado, but you can't relay the warning because you can't access the system. That's not hypothetical—that's exactly what would have happened if EAS had been cloud-dependent during Monday's outage.

My take: on-premise EAS hardware should remain the foundation even as internet-based capabilities expand. CAP and IPAWS are valuable *supplements* that extend reach and provide detailed information. But during catastrophic infrastructure failures—exactly like what happened Monday—traditional broadcast-based EAS provides the reliability that life-safety systems require. Making cloud-based EAS the *primary* system puts lives at risk when providers inevitably fail.

## The Monoculture Problem

What Monday really exposed is what Plummer calls "[internet monoculture](https://www.wired.com/story/what-that-huge-aws-outage-reveals-about-the-internet/)"—too many critical services concentrated on too few massive providers. AWS, Azure, and Google Cloud run huge portions of the internet. When one fails, the blast radius is enormous because everything depends on the same infrastructure.

Broadcast infrastructure *can* provide diversity. RF signals require only transmitters, towers, and power—no DNS, no API calls, no cloud dependencies. But modern stations increasingly depend on cloud services for automation, traffic, and content management. That's fine as long as we're not putting everything on one provider with no backup plan.

If AWS can experience hours-long outages—and it's one of the most reliable providers on Earth—any provider can fail. The question isn't *if* your cloud provider will go down. It's *when*, and whether you've architected your systems to survive it.

The fix is straightforward: treat cloud providers like internet providers. Have a primary and a backup. Test your failover regularly. Make sure your backup doesn't secretly depend on your primary (like having Lumen route through Spectrum's infrastructure—that's not real redundancy). For life-safety systems like EAS, keep the foundation on-premise and independent.

Monday's outage should be broadcasting's wake-up call. You wouldn't run a critical business on single internet with no backup. Don't run a radio station on single cloud with no backup. And definitely don't move emergency alerting to infrastructure that can fail when you need it most.