# How to protect your phone or laptop before sending it for repair: the 2026 checklist

*Guide · Apr 2026 · 10 min read*

> A 12-step pre-repair checklist for phones and Windows laptops, grounded in real incidents from Apple/Pegatron to Kolkata 2025. Backups, encryption, account hygiene, and forensic recording, in the right order.

**TL;DR** — Most laptop and phone repair privacy incidents would have been prevented (or at minimum produced evidence) if the customer had spent twenty minutes on a structured handover. This is the 2026 version of that checklist, including new steps that did not exist five years ago.

Most repair-shop privacy incidents are not catastrophic. They are small, opportunistic, and entirely preventable with twenty minutes of preparation. This is a working checklist for anyone about to hand a Windows laptop or a phone to a service centre, an in-house IT team, or a friend who will fix it.

The order matters. Skip the early steps and the later ones lose effect. The Apple/Pegatron, Kolkata, and Guelph cases (see [the catalogue](./phone-laptop-repair-shop-privacy-breaches-real-incidents.md)) all turn on access that one or more of these steps would have blocked.

## Phone-specific steps (skip if it is a laptop)

1. **Move sensitive media off the device.** Backup, then delete-from-device, then secure-empty if your phone supports it. The Kolkata and Trivandrum cases turned on intimate media that was on the device. If it is not on the device, the technician cannot copy it.
2. **Sign out of cloud accounts.** Google account, Apple ID, WhatsApp web sessions, Telegram cloud, banking apps. Not the device, the accounts.
3. **Set a temporary passcode.** Six digits, not your usual one. If the shop needs the device unlocked for testing, share this temporary one. Reset to your normal passcode when you get the device back.
4. **Enable Lost Mode awareness.** Apple Find My and Google Find Hub both let you remotely lock or wipe the device if something looks wrong during the repair window. Have the credentials ready on a second device.

## Laptop-specific steps (skip if it is a phone)

1. **Verified backup, not optimistic backup.** OneDrive showing a green tick is not a backup, it is a sync. Make a real, offline backup to an external drive, then restore one folder to a different machine to confirm it works.
2. **Sign out of every cloud account that auto-syncs.** Browsers, password managers, OneDrive, Dropbox, Google Drive. Anything that survives a reboot signed in is a credential exposure.
3. **Confirm BitLocker is on.** Settings, System, About, BitLocker. If it is off, turn it on at least 24 hours before the handover. BitLocker does not stop a powered-on, signed-in attack, but it makes a stolen drive useless.
4. **Save the BitLocker recovery key elsewhere.** A printed copy in a desk drawer is fine. If the technician changes the boot configuration during repair, BitLocker will demand the key on next boot.
5. **Create a separate, low-privilege technician account.** Do not hand over your daily-driver account. Create a local admin account named after the technician or service ticket. Sign in to that account during the handover. After the device returns, audit and delete it.
6. **Snapshot the system state.** Screenshots of: installed apps (Settings, Apps, Installed apps), services running (Get-Service in PowerShell), startup entries (Task Manager, Startup apps), and your system tray. After the device returns, diff these.
7. **Install [Black Box](https://www.alcyonesecure.com/products/blackbox).** Forensic recorder, 2.9 MB, signed installer, free for individuals. It logs USB events, file accesses, logins, and process starts into a SHA-256 hash chain. If the device is tampered with, you will know; if it is not, you will have a clean record to that effect.
8. **Document the device condition.** Photograph the keyboard, screen, and casing. Removes ambiguity if the device returns with new wear that the shop denies.

## Common steps (always do)

1. **Tell the technician you are recording.** Optional but useful. A bench that knows it is recorded behaves differently. A reputable shop will not object; an unreputable one might. Either signal is informative.
2. **Get a written work scope.** Ask the shop to write down what they intend to do, what parts they intend to replace, and what data access they expect to need. Not forensic evidence, but a commitment that constrains scope creep.
3. **Audit on return.** Compare snapshots, generate the forensic report from Black Box, look for: new admin accounts, new startup entries, USB devices you did not recognise, file accesses outside the work scope, and time-source changes. Most of the time everything will be clean. When it is not, you have evidence.

## What this prevents and what it does not

This checklist makes opportunistic snooping much harder, makes incidents detectable, and produces evidence usable in a dispute. It does not stop a determined attacker with kernel access and time. For most repair scenarios, including all the cases in our [incident catalogue](./phone-laptop-repair-shop-privacy-breaches-real-incidents.md), it is the right defence.

> **The price of confidence** — Twenty minutes before the handover. Five minutes after the device returns. That is what prevents most of the documented privacy breaches in the repair industry.

## What changed in 2026 vs the 2024 version of this list

Three steps are new this year:

1. **Lost Mode awareness for phones.** Apple and Google both expanded their out-of-band lock and wipe controls in 2025. They are now usable in real time during a repair window.
2. **Temporary passcode pattern.** Common in 2026, less so two years ago. Reduces credential exposure even when the device must be unlocked.
3. **Forensic recording on Windows is now consumer-grade.** Until 2025, this was an enterprise-only capability. [Black Box](https://www.alcyonesecure.com/products/blackbox) brings the same primitives to home users without a per-seat fee.

**Q: Do I really need all 12 steps?**

If the device is your daily-driver and contains personal media, banking sessions, or work accounts, yes. If it is a clean spare with nothing on it, the laptop-specific snapshot and forensic recording steps are still worth doing because they are cheap and produce evidence.

**Q: Will installing Black Box void my warranty?**

No. It is a normal Windows service that runs in the background. It does not modify the operating system, does not require any boot-level changes, and is digitally signed.

**Q: What if my repair is at an OEM-authorised service centre, not a small shop?**

The Apple/Pegatron case in 2016 happened at an authorised contract facility. OEM authorisation is not a substitute for the per-device defence. The checklist still applies.

**Q: How long does this whole process take?**

About 20 minutes before handover and 5 minutes after the device returns. Less if you do this often and have the snapshots scripted.

**Q: Is this overkill for a routine repair?**

If you are confident the device contains nothing sensitive and you are happy to bear the risk if it does, you can skip the snapshot and recording steps. The first six steps (the data-hygiene ones) take five minutes and are worth doing every time.

---

*Published on the [Alcyone Secure blog](https://www.alcyonesecure.com/blog/windows-laptop-pre-repair-checklist). This document mirrors public website content for open, offline, and machine reading.*
