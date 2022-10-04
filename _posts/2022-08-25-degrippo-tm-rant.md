---
layout: post
title: About DeGrippo's Treat Modeling rant
date: 2022-08-25 21:21:21 +0530
tags:
- threatmodeling
- cybersecurity
- rant
---

I stumbled upon [Sherrod DeGrippo](https://www.linkedin.com/in/sherroddegrippo/)'s [rant on Twitter about Threat Modeling](https://twitter.com/sherrod_im/status/1563199887096696832), claiming that it's BS.

Here are my thoughts about it:

Although it has caused quite a stir in the [Threat Modeling (TM) community](https://app.slack.com/client/T04T40NHX/C1CS3C6AF), I think she made some fair points:

1. Lack of standardisation of classical TM approaches leads to statements like "my threat model is not your threat model" without any further explanation of how they have reached that conclusion. 
2. Usually, TM doesn't take into account Cyber Threat Intelligence (CTI) input which translates into poor risk management.
3. There is a communication gap between the business objectives and the security implications to fulfilling them.

That said, here are my two cents:

- We need to find a balance between standardisation and flexibility. The ultimate TM standardisation would be a static cheat sheet, but that's far from optimal. On the other hand, too much flexibility might result in a lack of replicability, which can decelerate the adoption of TM, IMHO.
- Some degree of flexibility is a must since we need to implement the TM practices into a specific technical and business context. However, I agree that "there are no silver bullets" kind of statements can fall into an authority fallacy if they're not backed up with a proper explanation.
- From my experience, CTI plays a critical role in TM. Note that input isolated doesn't make any difference, we should make decisions based on that data, and that is... oh, a threat model! You are implicitly addressing the questions of the TM manifesto. On a side note, the 4th phase of PASTA (a risk-centric TM methodology) is about this topic.
- If you only pay attention to CTI, how do you secure brand new software releases (e.g. mobile app)? What about those raising trends that haven't affected your org yet? That is a reactive way of thinking that isn't compatible with a mature security program. 
- Common TM implementations assume the existing detection and prevention controls and often don't question the architecture decisions, which leads to securing stupid ideas rather than challenging the design. Again, this is also reactive.
- We must implement KPI, KRI and KCI to back up the effectiveness of TM and ultimately relate those metrics with the business objectives (SABSA layered approach can help with that) so the board don't get lost in translation.
- Despite the Security team being the owner of the TM practices, we should aim to embed TM in the org's SDLC and culture (a RACI matrix can help to set clear ownership). _Security is everyone's responsibility!_
