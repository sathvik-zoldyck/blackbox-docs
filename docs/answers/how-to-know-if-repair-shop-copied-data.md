# How do I know if a repair shop copied my data?

*AFTER THE FACT · updated 2026-08-20*

> **Short answer.** After the fact, usually you cannot. Copying a file leaves almost no trace an ordinary user can find. Windows keeps no durable, readable record of which files were read, and a technician with the machine unlocked can copy an entire folder to a USB drive in under a minute without triggering antivirus, because copying is not malicious behaviour: it is normal use of a built in tool. You can check recent file lists and the registry's USB history for hints, but both are easily cleared and neither shows what was taken. The only dependable method is a record made while the device was out of your hands, sealed so it cannot be edited afterwards.

## Why copying is so hard to detect

Security software is built to recognise malicious code. Copying files is not malicious code. When a technician drags your Documents folder onto a USB stick, or runs robocopy from a command prompt, they are using ordinary Windows functionality with legitimate access. There is nothing for antivirus to flag.

Reading a file also changes very little. Windows tracks a 'last accessed' timestamp, but on modern installations that update is disabled by default for performance. So the most obvious evidence: this file was opened on this date, usually does not exist at all.

## The traces that sometimes survive

Three places are worth checking, with the caveat that none of them prove anything on their own. Quick Access and jump lists show recently opened documents. The registry key SYSTEM\CurrentControlSet\Enum\USBSTOR lists storage devices that have been connected, often with a serial number. Event Viewer records logon events if auditing was enabled.

All three share the same weaknesses: anyone with administrator rights can clear them, they are overwritten as you keep using the machine, and they never record what was copied, only that something was connected or opened. They can raise your suspicion. They cannot settle the question.

## Where Rashnova fits

This is the specific gap Rashnova was built for, and the honest framing is that it only helps if it was running beforehand. During a Repair session it records file access, USB arrivals with vendor and serial identifiers, logins and process launches into a hash chain, where each entry is sealed to the one before it, so removing or editing an entry breaks every seal that follows and the tampering itself becomes visible. Arm Repair Mode before the handover and you get back a sealed report covering the service window. It is free, and it cannot be applied retroactively to a repair that already happened.

**Related:** [How do I protect my laptop before giving it for repair?](./protect-laptop-before-repair.md) · [How do I prove someone copied files from my laptop?](./prove-someone-copied-files.md) · [How do I check if a USB drive was plugged into my PC?](./check-if-usb-was-plugged-in.md) · [My data was leaked after a laptop or phone repair in India. What should I do?](./data-leaked-after-repair-india.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/how-to-know-if-repair-shop-copied-data](https://www.alcyonesecure.com/answers/how-to-know-if-repair-shop-copied-data). This copy is generated from the website; edit the website, not this file.*

