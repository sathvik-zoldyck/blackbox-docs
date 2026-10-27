# The University of Guelph study: repair technicians snooped in 6 of 16 visits

*Investigation · Apr 2026 · 8 min read*

> **In short:** In a peer reviewed study (IEEE Symposium on Security and Privacy, 2023), University of Guelph researchers left new Windows laptops with a simple audio fault at 16 repair shops in Ontario. Technicians looked through personal data in 6 of the 16 repairs, half of the 12 whose logs could be read, and copied it to a USB drive in 2. Of the 6, 3 cleared Windows' recent files list afterwards and 1 left no trace at all.

Most arguments about repair shop snooping are anecdotal. A friend who knows a friend, a Reddit thread, a viral post. The University of Guelph study is different. Jason Ceci, Jonah Stegman and Hassan Khan published it as *No Privacy in the Electronics Repair Industry*, peer reviewed and presented at the IEEE Symposium on Security and Privacy in 2023. Part of it was an instrumented experiment: laptops that logged everything, left for a repair that had no reason to involve anyone's files.

It is the clearest measured evidence there is that snooping at the repair counter is a pattern, not a rumour.

## How the experiment was set up

The researchers bought new Windows 10 laptops and disabled the audio driver, so each one had a simple, cheap fault that needs no access to anyone's files. Six laptops were used, three set up as a man's and three as a woman's, each with:

- Email and gaming accounts, and browser history built up over several weeks.
- Documents and pictures of the experimenters.
- A cryptocurrency wallet with its credentials.
- Revealing pictures, used with the consent of the people in them.

A logging tool on each laptop recorded every action the technician took, and Windows' own audit policy logged access to every file. The laptops went to 16 repair visits in Ontario: two national chains, two regional chains and eight local shops, with national and regional chains visited at two branches each.

Fixing an audio driver does not require opening a single personal folder. Any look at photos, documents or browsing history during that job is snooping.

## What the data showed

Logs could be read from 12 of the 16 visits (two shops fixed the fault in front of the experimenter, and two left no usable logs). Across the 16:

1. **Technicians looked through personal data in 6 repairs**: half of the 12 whose logs could be read. Pictures folders and the revealing pictures were opened most often; documents, a finance folder and browsing history in some.
2. **In 2 repairs, data was copied to an external drive.** In one, the revealing pictures were zipped and copied; in another, the pictures and a file containing passwords.
3. **Of the 6, 3 covered their tracks** by clearing Windows' Quick Access and recently accessed files list, and 1 left no trace there at all by zooming in on thumbnails instead of opening the files.
4. **The laptops set up as a woman's were targeted more often.**

> **What the study does and does not say** Sixteen visits in one Canadian province is a small sample, and the authors say so. It does not tell you the odds at your shop. It tells you something more useful: snooping happens at big chains and small shops alike, it is aimed at photos, and the people who do it often clean up after themselves. In the same study, 10 of 11 providers asked for full access to the device even when the repair did not need it.

## Why the study replicates so well in the wild

Three structural conditions explain why the Guelph result is consistent with later real world reports (the 2024 Singapore CNA Insider investigation, the 2025 Kolkata and Trivandrum incidents in India, the long Geek Squad pattern in the US):

### 1. The bench is unsupervised

Repair shops are not supervised environments. The technician is alone with the device. Access is opportunistic: a customer's Pictures folder is one click away, and the only thing stopping it is the technician's own restraint.

### 2. Windows does not keep a record of who opened what

By default, Windows does not audit file opens. The researchers had to switch that on themselves to see anything. The one trace an ordinary user might find, the recent files list, is exactly what three of the technicians cleared. So snooping is, by default, invisible to the customer and to the shop owner.

### 3. The customer cannot verify the work

Most customers cannot tell, post repair, whether their files were touched. They certainly cannot tell whether copies left the device. This is a market lemons problem: snooping shops look identical to clean shops, and the customer chooses on price.

## What changes when the device records the bench

The researchers could only see what happened because they had built the logging themselves. With [Rashnova](https://www.alcyonesecure.com/products/rashnova) in Repair Mode, an ordinary owner gets the same kind of record. A snoop like the ones in the study would have left:

1. The sign in when the technician unlocked the laptop, with its time.
2. Each file and folder opened, by name and path, sealed into the record so it cannot be quietly edited.
3. The USB drive, by maker and serial number, and every file copied to it.
4. Clearing the recent files list, recorded as someone covering their tracks.

When the laptop comes back, that is one report, with the findings first. The Guelph study did this for research. Rashnova does it for anyone with a Windows laptop, for free.

## Practical takeaways

1. **Do not assume your shop is the safe one.** Snooping turned up at national chains and local shops alike.
2. **Restrict the surface.** Sign out of cloud accounts, remove sensitive data, eject external drives before the handover.
3. **Record the session.** Install [Rashnova](https://www.alcyonesecure.com/products/rashnova) on Windows. The shop bench stops being anonymous.
4. **Audit on return.** Compare snapshots, run the forensic report, look for unauthorised opens, USB events, or process starts.

**Sources**

- [Ceci, Stegman and Khan, No Privacy in the Electronics Repair Industry (IEEE S&P 2023, arXiv 2211.05824)](https://arxiv.org/abs/2211.05824)
- [Help Net Security on the study](https://www.helpnetsecurity.com/2022/11/16/computer-smartphone-repair-data-privacy/)
- [Lifewire on the study](https://www.lifewire.com/need-a-computer-repair-study-finds-your-personal-data-may-be-at-risk-6890084)

## Questions

**Was the Guelph study peer reviewed?**

Yes. It was published as No Privacy in the Electronics Repair Industry by Jason Ceci, Jonah Stegman and Hassan Khan of the University of Guelph, and accepted at the IEEE Symposium on Security and Privacy 2023, one of the main peer reviewed conferences in computer security. The full paper is free on arXiv (2211.05824).

**Is it true that half of repair shops snoop?**

Not quite, and the difference matters. Technicians snooped in 6 of 16 repair visits. Logs could only be read from 12 of the 16, so it was half of the visits that could be checked. With a sample this small, the honest reading is that snooping is common enough to plan for, not that it is a fixed rate.

**Did the researchers identify the specific shops?**

No. The paper describes them only as national, regional and local service providers in Ontario. The point was to characterise the industry, not to single out businesses.

**Is snooping illegal?**

Accessing someone's data without their consent is an offence under most computer misuse and privacy laws, India's IT Act included, but cases are rarely brought, because the owner usually has no evidence. That is the gap a record made during the repair closes.

**Can I install monitoring on my own laptop without telling the shop?**

On a laptop you own, yes. Recording your own device is not surveillance of a third party. Some jurisdictions require notice if you intend to use the recording in a legal proceeding involving the technician; check local rules. As a courtesy, telling the shop is also a useful filter, an honest shop will not object.

---

*Source of record: [https://www.alcyonesecure.com/blog/guelph-study-half-repair-stores-snoop-on-customers](https://www.alcyonesecure.com/blog/guelph-study-half-repair-stores-snoop-on-customers). This copy is generated from the website; edit the website, not this file.*

