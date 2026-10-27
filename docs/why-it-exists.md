> This page mirrors [Why Rashnova exists](https://www.alcyonesecure.com/why) on alcyonesecure.com, the source of record.

# I asked where the photographs *were coming from.*

Most of us have done it without thinking. You hand a laptop or a phone across a counter. You watch someone write your name on a slip of paper. You walk out.

For the next day or two, a device holding your photographs, your messages, your bank details and your work sits in a room you will never see, in the hands of a person you will never meet again. You trust them, because there is no real alternative on offer. And you have almost no way of knowing what happened while it was gone.

A few years ago, before any of this was a company, a friend and I were tracking channels on [redacted] that were distributing stolen private photographs of women. We reported channels. New ones appeared the next day. The work was slow and mostly futile, and it went on long enough that I stopped expecting it to lead anywhere.

One night I asked one of the operators a direct question: where do these images actually come from?

He listed three sources. The first two I had expected.

> Repair shops.

He described technicians who copied customer drives before performing the repair. Photographs. Videos. Personal files. The material was sold. The owners never knew.

I had read the reports. I had seen the studies, the University of Guelph field test, the Apple settlement, the cases we now keep on file. I understood the pattern in the way you understand a statistic. Hearing it stated casually by someone inside that economy made it concrete in a way no statistic ever had.

What stayed with me was not the operator. It was the ordinariness of the other end. Parents, students, professionals, walking into ordinary shops on ordinary afternoons, with no reason to suspect that a device handed over for a cracked screen could become a permanent exposure.

I went looking for a tool that would let an ordinary person keep an independent, tamper evident record of what happened to their device while it was outside their control. Fully local. Owner-controlled. Cryptographically verifiable. No hidden telemetry, no content capture. I could not find one that met those requirements. So I started building it.

The honest version of what followed: it took place in a small room with limited resources. There were long stretches of research, several approaches that did not work, and periods where progress was hard to see at all. People who were part of the early effort moved on, which was reasonable of them. There were points where stopping would have been the rational decision. I kept going because the original problem had not gone anywhere.

## What it became

Rashnova is a forensic recorder for Windows. It runs quietly in the background from the moment you install it, keeping a hash chained, encrypted record of the activity on your machine: file access, process execution, USB connections, logins, and certain critical changes. The log is built so that any attempt to alter it becomes mathematically visible.

It started as something you switched on before a handover. It is not only that any more. Most weeks nothing happens to your computer, and you should still be able to check, so it also hands you a plain weekly summary of what your machine actually did, and a thirty second scan for the moments when something feels off. Before you hand the device to anyone, Repair Mode seals the whole window into a report you can give to a third party.

It does not capture keystrokes, screen contents, passwords, or the files themselves. **It records metadata about activity, not the content of your life.** The logs stay on your device, encrypted with a key we never hold. Which means we cannot read them, and could not hand them over if we were asked to.

## Why the recorder is free

This is not an antivirus product. Antivirus is built to detect malicious software. Rashnova is built for a different situation: when the risk is a person with legitimate physical access to the machine.

The people who face that risk most often: women, students, parents, freelancers, anyone who has to occasionally trust a device to a stranger, should not have to pay to keep basic evidence of what occurred. So the recorder is free for individuals, permanently, and it was free from the first version rather than as a growth tactic. The company is funded by organisations that need compliance evidence and fleet management. Individuals fly free.

We do not partner with repair businesses, and we will not. The product works for the owner of a device, not for whoever is temporarily holding it, and an arrangement with the second group would quietly corrupt our obligation to the first. If a shop chooses to run the free version to show its customers what it did, that is their decision and it still serves the owner. That is a different thing from a partnership.

If you have ever handed a machine to someone else and later wondered what actually took place: this was built for that moment. And for the ordinary Tuesdays in between, when nothing happened at all and you would simply like to know it.

## Commitments, stated plainly.
- **We will not read your files.** Files opened by us: zero. Logs are encrypted on your device.
- **We will not hold a key that opens your logs.** Keys never leave your device. We could not comply with a demand to decrypt, because we physically cannot.
- **We will not sell or share what the recorder sees.** Records sold: zero. This survives any change of ownership: it is written into our terms.
- **We will not put advertising in the product.** Not now, not at any scale.
- **We will not phone home unasked.** Nothing from your record is ever sent. The app makes two small requests that carry nothing from it: a daily check for a newer version, and, during a session, a check of the time.
- **We will not partner with repair businesses.** It would compromise the only thing that makes this worth using.

IF ANY OF THOSE EVER CHANGES, YOU HEAR IT FROM US FIRST · PUBLICLY.

---

*Source of record: [alcyonesecure.com/why](https://www.alcyonesecure.com/why).*
