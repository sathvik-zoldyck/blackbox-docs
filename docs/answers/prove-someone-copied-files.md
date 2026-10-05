# How do I prove someone copied files from my laptop?

*EVIDENCE · updated 2026-08-20*

> **Short answer.** Proof needs three things: a record created at the time, evidence that the record has not been altered since, and enough detail to identify what was taken and by which account. A screenshot satisfies none of them: it can be edited, and it only shows a moment. Windows' own logs are not built to be evidence: they can be cleared by an administrator and they rarely record file reads at all. What holds up is a log written as events occur and cryptographically sealed, so any later edit is detectable. A hash chain does this, each entry contains a hash of the previous one, so altering an entry breaks every hash that follows.

## What makes a record count as evidence

Rules of evidence differ by jurisdiction, but the questions asked of a digital record are broadly consistent. When was it created, at the time of the events, or reconstructed afterwards? Can it be shown not to have been altered since? Is it clear where it came from and who handled it? And does it actually record what is being claimed?

Most things people bring to a dispute fail on the first or second question. A photograph of a screen is a reconstruction. A copied log file has no integrity property, nothing distinguishes the original from an edited version. This is not a technicality; it is the whole reason tamper evidence exists as a concept.

## How hash chaining changes it

A hash chain works like this: every log entry includes a SHA-256 hash of the entry before it. Change one character in entry 40 and its hash changes, which means entry 41's stored hash no longer matches, and so on to the end of the file. You cannot quietly edit the middle. You cannot delete a line without leaving a break where the chain stops matching.

That converts integrity from a promise into a property of the file itself. Anyone can verify it independently, without trusting you and without trusting the software vendor, by recomputing the hashes.

## The limit worth stating plainly

Tamper evidence proves a record was not altered. It does not, by itself, prove that the record was accurate when written, and it is not a substitute for legal advice about your specific situation. Admissibility depends on your jurisdiction and the facts of the case. What a sealed log gives you is a far stronger starting position than a memory or a screenshot.

## Where Rashnova fits

Rashnova produces this kind of record. It logs file access, USB device arrivals with vendor and serial identifiers, logins and process execution with command lines, and seals each entry into a chain as it is written. Reports export as PDF, web page or spreadsheet today, and evidence bundles that a third party can check offline are coming. An encrypted off device copy is coming with the paid plan, which matters because a local only record can be destroyed along with the device. As above: it has to be running before the events you want to prove.

**Related:** [How do I know if a repair shop copied my data?](./how-to-know-if-repair-shop-copied-data.md) · [How do I check if a USB drive was plugged into my PC?](./check-if-usb-was-plugged-in.md) · [How do I protect my laptop before giving it for repair?](./protect-laptop-before-repair.md) · [What is an evidence layer in cybersecurity?](./what-is-an-evidence-layer.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/prove-someone-copied-files](https://www.alcyonesecure.com/answers/prove-someone-copied-files). This copy is generated from the website; edit the website, not this file.*

