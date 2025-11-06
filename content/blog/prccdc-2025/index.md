---
title: "🛡️ Inside the Cyber Arena: Our Experience at PRCCDC 2025"
description: "Discover how the experience at PRCCDC 2025 was for BC InfoSec Club and why you should join us."
summary: "Learn about our journey at PRCCDC 2025, our achievements, and how you can be part of the action."
date: 2025-03-15T00:00:00+00:00
lastmod: 2025-03-16T00:00:00+00:00
draft: false
weight: 50
categories: [event, competition]
tags: [PRCCDC, cybersecurity, InfoSec Club, competition]
contributors: [Liam Dale]
pinned: false
homepage: false
seo:
  title: "Inside the Cyber Arena: Our Experience at PRCCDC 2025"
  description: "Explore the highlights and achievements of the BC InfoSec Club at PRCCDC 2025."
  canonical: "" # custom canonical URL (optional)
  robots: "" # custom robot tags (optional)
---

![PRCCDC Logo](images/PRCCDC_White.png)

Ever wondered what it’s like to defend a network against live hackers in real time? Our cybersecurity club just got back from PRCCDC 2025, one of the most intense and exciting cybersecurity competitions we've ever attended—and we want to tell you all about it.

## 📍 What is PRCCDC?

- PRCCDC stands for the Pacific Rim Collegiate Cyber Defense Competition.
- The PRCCDC is part of the larger CCDC (Collegiate Cyber Defense Competition) series, a national cybersecurity competition.
- The PRCCDC encompasses colleges from Washington, Oregon and Idaho.
- The PRCCDC simulates a blue teaming (cyber defense) exercise.
  - Colleges are in charge of their own infrastructure (11 VMs) and are expected to keep the services running on them throughout the two day competition, with the primary goal of avoiding compromise by the Red Team.
  - There are also 'injects' or simulated memo's from management which we were expected to complete during the event to garner points.
  - We also had a phone and discord chat we were expected to respond to formally and avoid pitfalls of scammers.
  - Additionally, we were expected to present the board of directors for our company.

## ⚡ TL;DR
- We competed at PRCCDC 2025, a cyber defense competition.
- Managed 11 VMs while under Red Team attack.
- Encountered wild scenarios (IRS calls, raccoon kidnappings).
- Learned a ton. Had a blast. We want *you* on the next team.

## 🎯 Our Mission

Ultimately our goal for this event was to expose club members to the wealth of events that the field of cybersecurity offers. Every week there is a CTF or competition being held, while we certainly didn't excel at the competition this year, we plan to come back in 2026 with even more experience and preparedness.

## 🧩 What We Learned

- Working in a live environment is way harder than expected. You think you know how to do things but quickly get in the weeds once you try to do something you thought was simple.
- Communication was an underlooked aspect of our team. Getting through this event requires good coordination by teams.
- We gained valuable knowledge in learning about IPS / IDS / SIEM systems to come back better prepared to install them on our network.
- Coming with hardening scripts would have gone far for our team. Other colleges brought with them tools which proved invaluable at getting their networks hardened quickly.

## 🛡️ The Experience

### Day One

The PRCCDC started pretty early for our team members, we all left our homes early Friday morning to get to Lacey, Washington around check-in at 7am. Needless to say we were all pretty groggy for the events of that day.

To prepare for the competition, our team printed out a stack of cheat sheets covering over a dozen different technologies—everything from Linux permissions to firewall rules.

The event itself started with a breakfast where the organizers of the PRCCDC went over the expectations of the day. We were handed packets containing obfuscated information about the network we’d soon be managing.

Then at 9am on the dot we were shuffled into our own room with desktops already setup, we were allowed to use our phone to log into the discord and then were expected to hand them off to the room judges at the front of the room.

From 9am to 6pm, we logged into our network, patched vulnerabilities, changed passwords, and tried to bail water out of the leaky ship we were now captaining.

We captained such robust machines as Hannah Montana OS:

![Hannah Montana Linux desktop.](images/hannahmontana.png)

And a RedStar OS instance, a linux distro hailing from North Korea of all places:

![RedStar OS interface, our North Korean workstation.](images/redstar.png)

> Periodically throughout the day we were tasked with answering phone calls from a variety of different characters. Some trying to order pizza, others trying to register bug bounties, and of course the IRS. 🙄

We also got familiarized with a fellow employee, one Mr. Macnibbles.

![The one the only, MacNibbles. Chatting with us in discord.](images/macnibbles.png)

We stayed near the top of the leaderboard for most of the day—then Icarus’d hard, soaring early and crashing even harder by mid-day.

Unknown to us by mid-day we'd already been compromised by the Red Team as they **exploited a day-zero on our domain controller**. Giving them in-plain text our password and subsequently the rest of our network. Though they weren't supposed to do any real damage until the second day, **our data was captured and scored** by the Red Team.

We closed out the day with some words of encouragement from the staff. 😔

### Day Two

On the second day better prepared we tackled the day, trying harder to clamp down on our network security.

As we dutiously worked on our network and injects, we were once again interrupted by an old man trying to inflate the wooden wheels on their wagon cart, attorneys at law and of course homeland security.

We managed to stop the Red Team a little better this day, but by 2pm our domain controller `crazy` was completely compromised. Mid-repair by one our team members the screen abruptly cut out, Windows restarted and we were greeted by **a completely trashed Windows install**, icons missing, a non-functional start menu. And then it blue screened. 😱

We prepared a presentation for the higher-ups, touting our network security policy and the types of attacks we were 'working' to mitigate.

> We also witnessed the complete saga of our company beginning to sell **raccoon meat pizza**, Mr. Macnibbles getting kidnapped, a raccoon disguising as Macnibbles take his place and the anti-climatic conclusion of Macnibbles returning from lunch at 4pm. 🦝

Our team slowly lost sanity as one of our team members drew increasingly detailed images of a raccoon, eventually ending up with masterpiece that is Thaddius:

![The complete version of Thaddius in the flesh.](images/thaddius.png)

> When all was said and done the up-time leaderboard resembled that of a bloodbath, no teams made it out of day 2 unscathed.

### Day Three

Day three ended off the competition with a recap of the event. We learned in greater details the layout of our network, got appreciation for our team's artistry and gained the perspectives of the Black Team (Infrastructure and Organizers), Orange Team (Scammers, Legitimate Customers and Macnibbles), Red Team (Attackers). Closing out the day with the final leaderboard and top 3 teams of the competition.

![Slide showing the layout of our network.](images/netlayout.jpg)

![Picture of our raccoon artwork on the black team's slides.](images/our-teams-artwork.jpg)

## 🙌 Why You Should Join InfoSec Club

> Whether you're a seasoned hacker or just curious about cybersecurity, our club welcomes everyone. We train together, laugh a lot, and take part in events like PRCCDC that put our skills to the test. You’ll never get this kind of hands-on experience in a classroom.

> We plan to go at the competition again next year, be part of our team and help us move to the national stage!

## 📢 Get Involved

- 💬 Join our [Discord!](https://discord.com/invite/8YKrvbcZyd)
- 📅 Visit our [weekly meetings during Bellevue College academic quarters! Online too!](https://bcinfosec.club/)
- ❓Message @ligeria with questions on Discord!

## 🎤 Final Note

Huge shoutout to Rod Pascaul for helping us coordinate this event, the PRCCDC organizers which created such a fun environment for us to compete in, and for those in the club who got to participate this year! Can't wait to join next year's PRCCDC with y'all!

![Picture of our PRCCDC InfoSec Club Team.](images/group-pic-prccdc2025pic1.jpg)

![Picture of our PRCCDC InfoSec Club Team.](images/group-pic-prccdc2025pic2.jpg)
