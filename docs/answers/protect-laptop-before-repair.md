# How do I protect my laptop before giving it for repair?

*BEFORE A HANDOVER · updated 2026-09-30*

> **Short answer.** Do five things, in order. Back up everything and check the backup actually opens, because repairs sometimes wipe drives. Sign out of every account that syncs automatically: browsers, password managers, cloud drives: because a signed in session is reachable by anyone at the bench without a password. Give the technician a separate Windows account rather than your own. Photograph the machine and note its serial, so a swapped part is arguable later. And keep a record of what happens while the device is out of your hands, because without one you are relying on trust alone. Do not rely on deleting files: deleted files are frequently recoverable.

## Why the usual advice is incomplete

Almost every guide to this question gives you the same three steps: back up, delete sensitive files, factory reset. Those are reasonable, but they share a blind spot. They all try to reduce what is on the machine, and none of them tell you what actually happened once it left. Long checklists have a second problem: people skim them. Five steps someone finishes are worth more than twelve they abandon.

That matters because most repairs need the machine powered on and unlocked. A technician replacing a screen or a battery has to boot it to test the work. At that moment your encryption is not protecting anything, your browser sessions are live, and your files are one click away. Reducing exposure is worth doing. It is not the same as knowing.

## What the research actually shows

A 2022 University of Guelph field study took laptops to sixteen repair shops for a simple battery replacement. Technicians accessed personal data at six of them. In 2021, Apple settled with a customer after contractors at a repair facility posted her private photographs to social media.

The point is not that most technicians are dishonest, the overwhelming majority are not. The point is that a shop that behaved perfectly and a shop that copied your photos hand you back an identical laptop. Without a record, you cannot tell which one you used.

## The checklist

1. **Back up first, and verify the backup opens.** Repairs sometimes involve reimaging a drive. Copy to an external disk or a cloud account, then actually open a few files from the backup before you hand anything over.
2. **Sign out of everything that syncs.** Browser profiles, password managers, OneDrive, Google Drive, Dropbox, messaging apps. A live session is a credential: it survives a reboot and needs no password to use.
3. **Create a temporary account for the technician.** Give them a separate Windows account with only what the repair needs, rather than your daily one. It does not stop an administrator, but it means routine work never touches your profile.
4. **Photograph the machine and note the serial.** Screen, casing, ports, and the serial number. Cheap insurance against a swapped part or a disputed scratch.
5. **Keep a record of the service window.** Decide in advance how you will answer the question 'what happened while it was gone?'. This is the only step that has to be set up beforehand, a record cannot be created after the fact.

## Where Rashnova fits

Rashnova is one way to do the fifth step. It is a free Windows recorder that runs in the background and logs file access, USB device arrivals, logins and process starts into a tamper evident hash chain. Before a handover you arm Repair Mode: every USB device and every file copied to one is recorded, and the whole service window is sealed into a report you get back. It does not prevent anything, the technician needs access to do the repair, and it will not tell you what is inside a file. It tells you what was touched, when, and by which account.

**Related:** [Should I wipe my laptop before giving it for repair?](./wipe-laptop-before-repair.md) · [How do I know if a repair shop copied my data?](./how-to-know-if-repair-shop-copied-data.md) · [Is it safe to give your laptop to a repair shop?](./is-it-safe-to-give-laptop-to-repair-shop.md) · [How do I prove someone copied files from my laptop?](./prove-someone-copied-files.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/protect-laptop-before-repair](https://www.alcyonesecure.com/answers/protect-laptop-before-repair). This copy is generated from the website; edit the website, not this file.*

