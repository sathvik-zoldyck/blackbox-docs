# The University of Guelph study: half of computer repair stores snoop on customers

*Investigation · Apr 2026 · 8 min read*

> How researchers at the University of Guelph proved (with tagged decoy files and battery-replacement requests) that roughly 50 percent of repair shops snoop on the customer files they have no reason to open.

**TL;DR** — University of Guelph researchers handed identical laptops to 16 repair shops asking only for a battery replacement (a job that requires no login or file access). Roughly half the shops opened tagged decoy files, browsed the camera roll, or copied data to USB drives. The study, covered by Lifewire and others, is the cleanest empirical evidence that repair shop snooping is structural, not a few bad apples.

Most arguments about repair-shop snooping are anecdotal. A friend who knows a friend, a Reddit thread, a viral X post. The University of Guelph study (covered by Lifewire and several Canadian outlets in 2022) was different: it was an instrumented experiment with control conditions, tagged data, and a job that had no legitimate reason to involve customer files at all.

The result is the clearest empirical proof we have that the snooping problem is structural.

## How the experiment was set up

The researchers used identical Asus laptops, factory-fresh, then loaded with a profile designed to attract attention from a curious technician:

- A folder of personal-looking photos.
- A browser history showing dating-app logins, banking sessions, and email.
- A folder of innocuous documents (CVs, tax stubs).
- A few intentionally provocative file names in the Pictures directory.

All files were tagged with last-access times. Forensic logging was enabled on each laptop so the researchers could see exactly which files were opened, when, and for how long. To make the test as conservative as possible, the work request was always identical: replace the battery.

Replacing a battery on most laptops does not require the technician to log in. It does not require the technician to access the file system at all. Any file access on a laptop sent for a battery replacement is, by definition, snooping.

## What the data showed

Across 16 shops:

1. Roughly half of the shops accessed customer files. Tagged photos were opened. Browser history was viewed.
2. In some shops, files were copied to USB drives. The forensic log captured the USB device VID, PID, and serial number, plus the file-copy events.
3. In a smaller subset, technicians attempted to open files that required password entry, suggesting curiosity rather than just casual browsing.
4. Across the entire sample, no shop had a documented reason to access the files. The job was always battery replacement.

> **The structural conclusion** — The Guelph study was not a study of bad shops. It was a randomly chosen sample of regular shops. The fact that snooping was observed in roughly half of them suggests the prevalence is much closer to a coin flip than to a rare event.

## Why the study replicates so well in the wild

Three structural conditions explain why the Guelph result is consistent with later real-world reports (the 2024 Singapore CNA Insider investigation, the 2025 Kolkata and Trivandrum incidents in India, the long Geek Squad pattern in the US):

### 1. The bench is unsupervised

Repair shops are not surveilled environments. The technician is alone with the device. Access is opportunistic: a customer Pictures folder is one click away, and the only deterrent is the technician self-restraint.

### 2. Stock operating systems do not log file opens

Default Windows audit policy does not record file-open events. Default macOS audit is similar. Phones offer even less. So the snooping is, by default, invisible to the customer and to the shop owner.

### 3. The customer cannot verify the work

Most customers cannot tell, post-repair, whether their files were touched. They certainly cannot tell whether copies left the device. This is a market lemons problem: snooping shops look identical to clean shops, and the customer chooses on price.

## What changes when the device records the bench

If the test laptop in the Guelph study had been running a forensic recorder of the kind we ship with [Black Box](https://www.alcyonesecure.com/products/blackbox), every snoop event would have produced four artifacts:

1. A login event when the technician unlocked the laptop, with timestamp.
2. A series of file-open events with full path, written into a SHA-256 hash chain.
3. USB device-arrival events with VID, PID, and serial, if a thumb drive was attached.
4. A process-start event for any copy utility (robocopy, xcopy, custom data-recovery tool).

All four artifacts are visible to the customer in a one-click forensic report. The Guelph study did exactly this in a research context. We made it a consumer product.

## Practical takeaways

1. **Assume snooping is a coin flip.** The Guelph data does not allow you to assume otherwise.
2. **Restrict the surface.** Sign out of cloud accounts, remove sensitive data, eject external drives before the handover.
3. **Record the session.** Install [Black Box](https://www.alcyonesecure.com/products/blackbox) on Windows. The shop bench stops being anonymous.
4. **Audit on return.** Compare snapshots, run the forensic report, look for unauthorised opens, USB events, or process starts.

**Sources:**
- [Lifewire on the University of Guelph study](https://www.lifewire.com/need-a-computer-repair-study-finds-your-personal-data-may-be-at-risk-6890084)

**Q: Was the Guelph study peer-reviewed?**

The original work was published as research from the University of Guelph and covered in mainstream tech outlets including Lifewire. Subsequent industry studies (notably from Consumer Reports and various security vendors) have replicated the qualitative finding without disagreeing with the headline number.

**Q: Did the researchers identify the specific shops?**

The published reporting de-identified individual shops. The point of the study was to characterise the industry, not single out vendors.

**Q: Is snooping illegal in most jurisdictions?**

Unauthorised access to a computer system without consent is generally an offence under most computer-misuse laws, but enforcement is rare and per-customer remedies are weak. The study was significant because it documented a baseline, which strengthens both regulatory and civil cases.

**Q: Can I install monitoring on my own laptop without telling the shop?**

On a laptop you own, yes. Recording your own device is not surveillance of a third party. Some jurisdictions require notice if you intend to use the recording in a legal proceeding involving the technician; check local rules. As a courtesy, telling the shop is also a useful filter, an honest shop will not object.

---

*Published on the [Alcyone Secure blog](https://www.alcyonesecure.com/blog/guelph-study-half-repair-stores-snoop-on-customers). This document mirrors public website content for open, offline, and machine reading.*
