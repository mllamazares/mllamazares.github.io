---
layout: post
title: Applying STRIDE to my hotel's minibar - Part II
date: 2022-09-26 21:21:21 +0530
tags:
- hacking
- threatmodeling
- riskmanagement
- evilpersonas
- cybersecurity
- humor
---

_This is the sequel of [Applying STRIDE to my hotel's minibar - Part I](/blog/stride-hotel-minibar-i)._

I wanted to make a quick note regarding risk appetite and evil personas.

Indeed, their hostel minibar's system is exposed to several types of threats. I used [STRIDE](https://en.wikipedia.org/wiki/STRIDE_(security)) as a baseline to help visualising the power of threat modelling in non tech-related contexts (big shout out to [Munzur](https://www.linkedin.com/in/munzur/) and [Therese](https://www.linkedin.com/in/theresedrent/), who plan to use this example in their upcoming workshops!).

However, we shouldn't just blindly start thinking about countermeasures without considering the business and environmental context. That is, are those threats actually an issue? What are the consequences of the worst-case scenario? Is the ROI of the countermeasures reasonable compared to the risk? Do we have data of past malicious events?, etc.

In other words, if the likelihood and criticality of those threats are low (minibar inside the hotel's compound, no records of past issues, the potential losses are widely compensated with the profits, etc.), why wasting our time and money designing a fancy electronic padlock system or assigning a waiter to administrate the drinks?

We tend to think about attackers like mythological creatures with endless resources and volatile motivations, but the reality is that there are various profiles, each with different level of expertise, objectives, preferred techniques, etc. 

Modeling evil personas is key to design mitigations that actually make sense within the org risk profile (industry, company size, country, infrastructure, data, competitors, roles, CTI feedback, etc.). IMHO, it's an essential variable when determining the likelihood of the attack and easing the security control's prioritisation.

**TL;DR** 

Sure, not taking security seriously might lead to catastrophic results, but, on the other hand, over securing our product might lead to a loss on competitive advantage. Thus, the 3rd question of TM manifesto ("what are we going to do about it?") must be strategically aligned with the amount of risk an org is willing to take in pursuit of their objectives (aka risk appetite). To do so, one powerful tool in our arsenal is modelling evil personas.

Finally, I'd like to reference the following related resources of my mate [Dave van Stein](https://www.linkedin.com/in/dvstein/):
- [Stop procrastinating failure! (YouTube)](https://www.youtube.com/watch?reload=9&v=Pt6iGUPYZXg) 
- [Start using Evil Personas (Xebia's blog)](https://xebia.com/blog/threat-modeling-start-using-evil-personas/)
