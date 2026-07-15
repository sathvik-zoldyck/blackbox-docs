# USB data theft: how 60 seconds and a thumb drive can copy your entire device

*Security · Apr 2026 · 7 min read*

> USB exfiltration is the most underrated threat in any unsupervised-device scenario. How it actually works, why standard antivirus misses it, and what kernel-level monitoring can do.

There is no safer-feeling moment in a repair shop than when the technician plugs in a thumb drive. It looks like a tool. It can be a tool. It can also be a one-minute exit door for everything on your machine.

USB-based exfiltration is the most consistently underrated threat in any unsupervised-device scenario, and it is one of the patterns the University of Guelph study (see [our analysis](./guelph-study-half-repair-stores-snoop-on-customers.md)) explicitly captured.

## How fast is fast

On a 2024-class laptop and a USB 3.2 Gen 2 stick, sustained sequential copy hits about 1 GB per second. A modest 256 GB drive can absorb the contents of an average personal laptop in well under five minutes. Robocopy and xcopy are part of stock Windows. There is no installer, no antivirus prompt, and no obvious trace once the drive is unplugged.

## Why antivirus does not catch it

Antivirus engines look for malware signatures and bad-behaviour patterns. A built-in Windows utility doing fast file reads is not malware behaviour. Some enterprise EDR products do detect bulk-copy patterns; almost none ship on consumer machines.

## What does work

- Kernel-level event tracing (ETW on Windows) that records process starts and file open volumes regardless of the API. This catches robocopy and xcopy at the level where they cannot hide.
- USB device-arrival logging with VID, PID, and serial number, plus matching device-removal records. Reconstructable timeline: a USB stick was here, between these two timestamps, while these files were being read.

Together, those two streams produce a forensic timeline. [Black Box](https://www.alcyonesecure.com/products/blackbox) runs ETW and the USB device watcher as part of its default event set. Each event is hashed into a SHA-256 chain, so a technician who reaches the log file cannot quietly delete the USB-arrival entry without producing a chain break.

## Practical hardening

1. Move sensitive files off the device entirely; they cannot be copied if they are not present.
2. Sign out of cloud accounts that auto-sync; otherwise a copied folder reaches a second host.
3. Run a forensic recorder, so any USB device that arrives is logged with VID, PID, and serial.

**Q: How long does a full-device copy actually take?**

On modern hardware with a USB 3.2 stick, around 1 GB per second sustained. The user profile of an average laptop transfers in under a minute.

**Q: Will my antivirus catch a robocopy bulk transfer?**

Almost certainly not on consumer Windows. Robocopy is a built-in administrative tool. Enterprise EDR products may flag it; consumer AV does not.

**Q: Does Black Box block USB devices?**

No. It records them. Blocking is a separate decision; recording is the evidence layer that makes the bench non-anonymous.

---

*Published on the [Alcyone Secure blog](https://www.alcyonesecure.com/blog/usb-data-theft-60-seconds). This document mirrors public website content for open, offline, and machine reading.*
