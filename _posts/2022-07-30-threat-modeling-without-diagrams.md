---
layout: post
title: Threat Modeling without diagrams?
date: 2022-07-30 21:21:21 +0530
tags:
- threatmodeling
- cybersecurity
- diagrams
---

So do you want to do Threat Modeling, but don’t have a diagram as an input?

Adam Shostack addresses this issue in a DEF CON [^1] talk called [_"The B-MAD Approach to Threat Modeling" (Youtube)_](https://www.youtube.com/watch?v=N5icvgTyg7k). B-MAD stands for _"**B**ring **M**e **A** **D**iagram"_, which is a recurrent phrase you hear from the Security team when they are entitled to analyse the threats of the system. However, from my experience, they frequently don't exist or are not updated, so treating them as a pre-requisite for threat modelling is a mistake — we need to be flexible. Thus, you know, if you cannot have a diagram as an input, don’t B-MAD.

On the technical aspect of the possible solutions, he proposed creating a _"Big Wall Map"_ (BWM) of the system that you could update whenever a feature impacts the architecture. It will enable a shared awareness to better answer the question _"What are we working on?"_, and most importantly, we don't necessarily need to create an ad-hoc diagram for each project.

Bear in mind that we should manage expectations and define clear ownership of who, when and how the diagram should be updated. My recommendation is to stick to a framework like [the C4 Model](https://C4model.com) by Simon Brown, which is developer-friendly and helps to standardise the level of detail (C2 or C3 should work fine in this context).

I see three potential improvements to the BWM approach:
 - It is not digitalized, therefore, not centralized. If your company has a WFH policy or has outsourced the development, that could be a drawdown.
 - You cannot keep track of the architectural changes. _"How was the architecture 16 months ago before we modified X service and migrated Y to AWS?"_.
 - It requires an initial investment of effort. Depending on the complexity and size of your codebase, that could be a bottleneck.

If we combine the BWM approach with Diagrams-as-Code (DaC), we could have a _living_ architecture diagram inside the repository. Their changes can be easily traced and associated with a specific modification of the code (same source of truth). 

Here are some DaC tools:
 - [Mermaid](https://mermaid.live/)
 - [Structurizr](https://structurizr.com/)
 - [Mindgrammer](https://diagrams.mingrammer.com/)
 - [PlantUML](https://plantuml.com/)

IMHO, diagramming should be considered basic hygiene. It plays a critical role in the design phase, and it has more benefits apart from threat modelling. 

> "The alternative to good design is bad design, not no design at all"
>
> -- **Douglas Martin**

---

[^1]: one of the world's largest and most notable hacker conventions, held annually in Las Vegas, Nevada.