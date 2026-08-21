# The software you installed is reading your Documents folder — and Windows will not tell you

*Investigation · Aug 2026 · 9 min read*

> Avast sold browsing data for six years. Lenovo shipped laptops that intercepted encrypted traffic. Neither was malware. What ordinary software does with your files, and why you cannot see it.

There is a particular kind of privacy failure that antivirus was never going to catch, because the software doing it is not malicious in any sense a scanner recognises. It is signed. It is popular. Often you paid for it. It simply does more with your data than it told you, and it does so for years before anyone notices — and when someone finally does, it is usually a regulator, not a user.

Two cases make the pattern concrete, and both ended in fines.

## The antivirus that sold what it promised to protect

In February 2024, the US Federal Trade Commission ordered Avast to pay **$16.5 million** and banned it from selling browsing data for advertising. The finding: since at least 2014, Avast had collected users' browsing information through its antivirus software and browser extensions, stored it indefinitely, and sold it to more than a hundred third parties through a subsidiary called Jumpshot.

The detail that matters is what the data contained. According to the FTC, it revealed users' religious beliefs, health concerns, political leanings, location, financial status and visits to child-directed content. And it was sold while Avast was telling users the product would block third-party tracking.

Six years. Millions of installations. Nobody running that software could see it happening, because there was nothing on their machine that would have shown them.

## The laptops that shipped with it already installed

In September 2017, Lenovo settled with the FTC and 32 state attorneys general for **$3.5 million** over VisualDiscovery — the Superfish adware preinstalled on consumer laptops. It used a man-in-the-middle technique that, in the FTC's description, allowed it to access all of a consumer's sensitive personal information transmitted over the internet: login credentials, Social Security numbers, medical information, financial and payment details.

The software was on the machine before the owner opened the box. There was no install to decline and no prompt to read.

## This is not a story about two companies

It would be comforting if these were outliers. Research published in January 2026 found that **64% of third-party applications access sensitive data without a demonstrable business need** — up from 51% the year before. Separate testing across mobile found that roughly 35% of iOS apps failed to disclose the data collection they were performing.

Enforcement is catching a little of it. The Texas Attorney General sued Arity over software embedded in hundreds of mobile apps that collected location and driving data from more than 45 million people and sold it on, including to insurers. But enforcement arrives years late, applies to a fraction of cases, and does nothing for the person who wanted to know what their own machine was doing last Tuesday.

## Why you cannot check this yourself

Windows has no view that answers "which programs have been reading my files?". The pieces exist, but none of them are usable by an ordinary owner:

- **Resource Monitor** shows live disk activity by process. Close the window and the information is gone — there is no history.
- **Sysinternals Process Monitor** captures everything in enormous detail. A quiet minute on an idle machine can produce fifty thousand events, and it is built for engineers debugging software.
- **File-system auditing** through Group Policy does produce a real audit trail, but it is off by default, must be configured folder by folder, is unavailable in some Windows editions, and writes to a log an administrator can clear.
- **The last-accessed timestamp**, which would be the obvious answer, is disabled by default on modern Windows for performance.

So the honest answer to "is this app reading my Documents folder?" on a stock Windows machine is: you cannot tell, and nothing is keeping a record that would let you tell later.

## What would actually help

Not detection. Nobody can reliably classify a file read as sinister — a backup tool and an exfiltration tool perform identical operations, and any product claiming otherwise is guessing. What helps is far more boring: **a durable, readable record of which program touched which folder, and when**, kept in a form the owner can review and nobody can quietly edit.

With a record like that, none of the cases above would have needed a regulator. Someone would have noticed their antivirus reading a great deal more than it needed to, and asked why.

This is what [Black Box](https://www.alcyonesecure.com/products/blackbox) does. It records file access at the kernel level into a hash-chained, tamper-evident log on your machine — which programs ran, which files and folders they touched, and when. It does not tell you an app is malicious. It keeps a record of what it did, which you can read and, if it matters, prove. It is free, and the log never leaves your device.

## Frequently asked

**Can antivirus detect software that reads too many of my files?** Generally no. Antivirus looks for malicious code and known-bad behaviour patterns. A signed, legitimate application reading files is normal operation — there is nothing for a scanner to flag. Both the Avast and Lenovo cases involved software that antivirus would have no reason to object to, in one case because it *was* antivirus.

**Was the Avast data anonymous?** The FTC described the browsing data Avast sold as detailed and re-identifiable, and found it revealed religious beliefs, health concerns, political leanings, location and financial status. Browsing histories are close to unique to a person.

**Does Black Box detect malicious software?** No, and it does not claim to. It is a recorder, not a scanner or a blocker. It keeps a tamper-evident record of what happened on your machine so you can see it and prove it. Detection is a different product category.

---

*Sources: [FTC order against Avast, Feb 2024](https://www.ftc.gov/news-events/news/press-releases/2024/02/ftc-order-will-ban-avast-selling-browsing-data-advertising-purposes-require-it-pay-165-million-over) · [FTC settlement with Lenovo, Sept 2017](https://www.ftc.gov/news-events/news/press-releases/2017/09/lenovo-settles-ftc-charges-it-harmed-consumers-preinstalled-software-its-laptops-compromised-online). Published on the [Alcyone Secure blog](https://www.alcyonesecure.com/blog/software-reading-your-documents-folder). This document mirrors public website content for open, offline, and machine reading.*
