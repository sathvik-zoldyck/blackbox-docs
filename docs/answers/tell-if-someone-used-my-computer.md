# How can I tell if someone used my computer while I was away?

*YOUR OWN MACHINE · updated 2026-08-20*

> **Short answer.** Windows keeps a few clues, none of them conclusive. Event Viewer records logon events in the Security log (event ID 4624) when auditing is enabled. Recently opened documents appear in Quick Access and in application jump lists. The registry keeps a list of USB storage devices that have been connected. Each of these can be cleared by anyone with administrator rights, none of them show what was read or copied, and several are overwritten as you keep using the machine, so checking a week later often finds nothing. They are useful for forming a suspicion quickly. A continuous, tamper evident record is what settles the question, and it has to be running beforehand.

## Where to look first

Start with Event Viewer: Windows Logs → Security, filtered to event ID 4624 for successful logons and 4625 for failed ones. Each entry carries a timestamp, an account name and a logon type, which distinguishes someone sitting at the keyboard from a remote session. If auditing was never enabled, this log will be sparse or empty.

Then check Quick Access in File Explorer, and the jump lists on your taskbar, right-click an application to see files it opened recently. Finally, Settings → System → Power shows recent sleep and wake behaviour, and the System log records startups and shutdowns under event IDs 6005 and 6006.

## Why none of it is proof

Everything above is designed for convenience or diagnostics, not evidence. Jump lists can be cleared in two clicks. The Security log can be wiped by an administrator, and wiping it is itself only recorded in the log you just wiped. USB registry entries can be edited.

There is also a subtler problem: absence of evidence is not evidence of absence. An empty jump list might mean nobody used your machine, or it might mean somebody cleared it. Without an integrity mechanism, you cannot distinguish a quiet week from an erased one, which is precisely the distinction that matters.

## Where Rashnova fits

Rashnova addresses the integrity problem specifically. Each log entry is sealed to the one before it, so deleting or editing any entry breaks every seal after it and the gap becomes visible rather than silent. Once you switch recording on it runs continuously, so there is no session to remember to start, and it produces a weekly summary of what your machine did. It is free and it stays on your device. The honest limit is the same as everything else on this page: it only covers time when it was already running.

**Related:** [How do I see which apps are accessing my files on Windows?](./see-what-apps-access-my-files-windows.md) · [How do I check if a USB drive was plugged into my PC?](./check-if-usb-was-plugged-in.md) · [What was my computer doing while I was asleep?](./what-was-my-computer-doing-overnight.md) · [How do I keep my privacy on a shared or family laptop?](./protect-privacy-on-shared-laptop.md) · [What free tools show what happened on my Windows PC?](./free-tools-see-what-happened-on-windows-pc.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/tell-if-someone-used-my-computer](https://www.alcyonesecure.com/answers/tell-if-someone-used-my-computer). This copy is generated from the website; edit the website, not this file.*

