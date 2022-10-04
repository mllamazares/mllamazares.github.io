---
layout: post
title: Applying STRIDE to my hotel's minibar - Part I
date: 2022-09-12 11:30:00 +0000
tags:
- hacking
- threatmodeling
- riskmanagement
- privacy
- pentesting
- cybersecurity
- humor

---

These holidays I've applied [STRIDE](https://en.wikipedia.org/wiki/STRIDE_(security)) to identify the threats to which the minibar of my hotel was exposed! 

Here's a high-level description of their system:

- The minibars are located in the common spaces (e.g. swimming pool). 
- If you feel thirsty, just grab a drink from the (unlocked) minibar and write it down in the corresponding column of the sheet (see picture below). 
- They use fruits (rather than numbers) to identify each room. 
- At the end of your stay, the hotel owners gather and review the sheets and charge the corresponding bill. 

![Minibar tracking system](/assets/images/stride-minibar.jpg)

OK, here we go with the threats:

- 🎭 **Spoofing**: grab a drink and write it down in a different guest room.
- 🤡 **Tampering**: drink a mineral water bottle and fill it in with tap water.
- 📝 **Repudiation**: steal a drink without writing it down in the sheet.
- 🔒 **Information disclosure**: track how many alcohol drinks guests have been taking lately (there is a privacy concern as it's quite easy to link each room with their guests).
- 💥 **Denial of service**: steal the sheet so guests can no longer record their drinks. The hotel owners must find an alternative solution quickly, and I bet there are no backups.
- 👑 **Elevation of privilege**: grab the sheet, put on a dress shirt, go to each room, and ask for cash pretending a change in the process [^1].

---

[^1]: By [Jonathan RAULT](https://www.linkedin.com/in/jonathanrault/)