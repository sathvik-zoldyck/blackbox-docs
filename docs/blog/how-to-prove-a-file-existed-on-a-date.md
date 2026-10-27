# How to prove a file existed on a certain date, and why your computer's date is not enough

*Guide · Oct 2026 · 9 min read*

> **In short:** The dates Windows shows on a file are notes the computer keeps for itself, and anyone with the file can change them. To show that a file existed, exactly as it is, by a certain time, you need three things: a fingerprint of its exact contents, a time witnessed by someone other than you, and a proof anyone can check without trusting you or the company that made it. Rashnova Proof does all three for free, on your own computer.

> **The short version** The date on a file proves nothing to anyone who doubts you. A fingerprint of the file, witnessed in time by independent services, does. You can make one for free, and your file never has to leave your computer.

You signed a lease. You photographed the flat on the day you moved in. You finished a design before you sent it to a client. Months later, someone says the lease was different, the scratches were already there, or the design was theirs first. You open the folder, point at the date beside the file, and realise it settles nothing.

This guide explains why, and what does settle it.

## Why the date beside a file is not proof

Windows keeps three dates for most files: when it was created, last changed and last opened. They are bookkeeping for the computer, not a record for anyone else. Copying a file to a new drive gives it a new created date. Free tools change all three in a few clicks. Even a perfectly honest date only tells you what your own computer believes, and your computer's clock can be set to anything.

Screenshots and email have the same weakness from a different side. A screenshot shows what a screen looked like, but it is easy to edit and carries no proof of when it was taken. An email to yourself shows that some text passed through a mail server, but attachments get forwarded, renamed and re saved, and the other side can fairly ask which version you mean.

What a doubter needs is not your word about the date. It is something they can check for themselves.

## Step one: a fingerprint of the exact file

A cryptographic fingerprint (a hash) is a short string computed from every byte of a file. Change one comma in a contract, one pixel in a photo, and the fingerprint comes out completely different. The same file always gives the same fingerprint, on any computer, with any standard tool. That is what lets a proof say *this exact file*, and not just *a file with this name*.

Rashnova Proof takes two fingerprints of every file, with two different standards, SHA-256 and SHA3-256. Both are public and widely used; using two means that a weakness ever found in one does not undo the proof. The fingerprints are made on your computer. The file itself never goes anywhere.

If you have never seen a fingerprint change, our [plain English guide to hashes and hash chains](./hash-chains-explained-non-cryptographer.md) shows it step by step.

## Step two: a time that someone else witnessed

A fingerprint proves which file. It says nothing about when. For the when, the fingerprint has to be shown to someone who keeps an honest clock and who is not you. If only you witness the time, you are back to your word against theirs.

Rashnova Proof asks four independent witnesses, and never asks us:

- **drand**, a public randomness beacon run by the League of Entropy, a group of independent organisations. It publishes a new random value at a fixed rhythm. Your proof includes one of those values, and since nobody could know it in advance, your proof cannot have been made before it appeared. This is the *not before* side.
- **DigiCert** and **Sectigo**, two independent time stamp authorities. Each signs your file's fingerprint together with the time, using the long standing internet standard for time stamps, RFC 3161. This is the *not after* side: the file existed by then.
- **Bitcoin**, through OpenTimestamps, which places the fingerprint in a public ledger that nobody can quietly rewrite. It usually confirms within a few hours, and the app tells you when it has.

Only a salted fingerprint ever leaves your computer, never the file and never its name. Even the witnesses cannot tell what you proved.

## Step three: a proof that checks itself, even without us

A proof you can only check on the website of the company that made it is a proof that dies with that company. So every Rashnova proof is one file that carries its own checker. Open it in any web browser, offline, drop in the original file, and it says *Matches* or *Does not match*. A plain text guide inside the proof gives the same checks with standard tools, for anyone who would rather trust nothing they did not run themselves.

Each proof is also signed twice: once with ECDSA, today's standard, and once with ML-DSA-65, a post quantum signature standardised by NIST, so the proof still stands if today's signatures are ever broken. A one page certificate goes with it, with six check words, a QR code anyone can scan to check it, and a seal drawn from the proof itself, so no two look alike.

There is a fuller explanation of the witnesses in [Four witnesses, never us](./four-witnesses-how-a-rashnova-proof-is-witnessed.md).

## What a proof shows, and what it does not

Honesty here matters more than anything else on this page.

- **It shows** that this exact file existed, unchanged, by a certain time, witnessed by independent services.
- **It does not show** who made the file, who owns it, or that what it says is true.
- **It does not promise** that a court will accept it. That is for a court to decide.

For people in India, it may help to know that Section 63 of the Bharatiya Sakshya Adhiniyam, 2023 asks for a certificate to go with an electronic record, and the certificate's form asks for the record's hash value, the same kind of fingerprint a proof is built on. Rashnova Proof includes facts sheets for India, the United States and in general, so a lawyer or an expert can see exactly what was done. They are facts, not legal advice.

## How to make one, in about a minute

1. Install [Rashnova](https://www.alcyonesecure.com/download), free for Windows 10 and 11.
2. Open **Proof** and drop in a file, several files, or a whole folder.
3. Wait a few seconds while the fingerprints are made and the witnesses answer.
4. Keep the proof file somewhere safe, and the certificate if you like a printout.
5. Months later, anyone can check it: you, the other side, a lawyer, a court's expert, with or without Rashnova.

Rashnova also writes each proof into your computer's own sealed record, and keeps an eye on the proved file: if it changes later, it tells you.

> **When to prove something** The day you sign a contract. The day you move in or move out. Before you send your work to anyone. Before a laptop goes in for repair. Proof is cheap before a dispute and impossible after one.

## Questions

**Can the created date of a file be changed?**

Yes. Copying a file changes it, and free tools can set any date you like. The dates Windows shows are notes your own computer keeps, so they do not prove anything to someone who doubts you.

**How can I prove a file existed on a certain date for free?**

Make a fingerprint of the file and have independent services witness the time. Rashnova Proof does this for free on Windows: it fingerprints the file on your computer, has the time witnessed by drand, DigiCert, Sectigo and Bitcoin, and gives you a proof anyone can check offline.

**Does my file get uploaded?**

No. Only a salted fingerprint is sent to the witnesses. The file and its name never leave your computer.

**Can someone check my proof without Rashnova?**

Yes. Each proof carries its own checker that runs in any browser, offline, and a step by step guide for standard tools. The official checker is also published on our site.

**Does a proof show that I made the file?**

No. It shows that this exact file existed, unchanged, by a certain time. It does not show who made it or owns it, or that its content is true.

**Read next**

- [Rashnova Proof: how it works](https://www.alcyonesecure.com/proof)
- [Where did this photo come from?](./where-did-this-photo-come-from-metadata-content-credentials.md)
- [Four witnesses, never us](./four-witnesses-how-a-rashnova-proof-is-witnessed.md)
- [Free vs paid proof of existence](../answers/free-vs-paid-proof-of-existence.md)

---

*Source of record: [https://www.alcyonesecure.com/blog/how-to-prove-a-file-existed-on-a-date](https://www.alcyonesecure.com/blog/how-to-prove-a-file-existed-on-a-date). This copy is generated from the website; edit the website, not this file.*

