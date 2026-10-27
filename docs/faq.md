# Frequently asked questions

78 answers about Rashnova and Alcyone Secure, in 9 groups.

- [What people ask most](#what-people-ask-most)
- [General](#general)
- [The recorder](#the-recorder)
- [Rashnova Proof & Origin](#rashnova-proof--origin)
- [Privacy & the cloud](#privacy--the-cloud)
- [Tampering & evidence](#tampering--evidence)
- [Legal & compliance](#legal--compliance)
- [Other products](#other-products)
- [Billing & support](#billing--support)

## What people ask most

*The questions people type about repair shops, their files and proving things, answered plainly*

### Can repair shops see my photos?

Yes, if the device is unlocked or they have your password, a technician can open anything on it, photos included. Most never do, but it happens: in a 2022 University of Guelph study, technicians looked through personal data in 6 of 16 repairs, half of those whose logs could be read, and copied it in 2. Before a repair, back up, sign out of cloud accounts, and give the shop a separate account instead of yours. Then keep a record of the visit: during a Repair session, [Rashnova](https://www.alcyonesecure.com/products/rashnova) notes every file opened and every USB drive plugged in, sealed so it cannot be quietly changed, and tells you when the laptop comes back. [Read the full answer](./answers/can-repair-shops-see-my-photos.md).

### Do computer repair shops look at your files?

Some do. Most repairs never need your files, yet studies and court cases show technicians opening photos and documents that had nothing to do with the fault. You usually cannot tell afterwards, because Windows does not keep a readable record of which files were opened. The fix is to record the visit while it happens: Rashnova's Repair Mode keeps a sealed account of what was opened, copied and plugged in, with plain findings and a verdict when the laptop is back. It is free.

### Should I remove my hard drive before sending my laptop for repair?

If the repair does not involve the drive (a screen, a keyboard, a hinge) and your laptop lets you remove it easily, yes: no drive, no data to see. Many modern laptops have the storage soldered to the board, so that is not always possible, and some repairs need the drive to test the machine. When the drive has to go with it: back up, move your most private files off, give the shop a separate account, and record the visit with Rashnova's Repair Mode so you know exactly what was touched. [Read the full answer](./answers/should-i-remove-hard-drive-before-repair.md).

### Should I give my password to the repair shop?

Not your own. Make a separate Windows account for the technician (Settings, Accounts, Other users), give them that password, and remove the account when the laptop is back. If the shop insists on yours, change it straight after. A separate account keeps your own files and signed in apps out of easy reach, though an administrator can still reach everything. That is why it helps to start a Repair session in Rashnova before you hand it over: anything done to your files gets written down and sealed.

### How can I tell if someone accessed my files on my laptop?

Windows gives you hints, not a record: Recent files in File Explorer, files sorted by date modified, and sign ins in Event Viewer. All of them can be cleared, and none says reliably who opened what. To know for certain next time, the record has to be running beforehand: [Rashnova](https://www.alcyonesecure.com/products/rashnova) keeps a sealed record on your own computer, free: always on, the things that matter, such as USB drives and sign ins; during a Repair or Handover session, every file opened and program started too. Any attempt to edit it shows. [Read the full answer](./answers/tell-if-someone-used-my-computer.md).

### How do I see what files were copied to a USB drive?

Windows does not keep that list. It remembers which USB drives were plugged in (in Device Manager with hidden devices shown, and in the registry under USBSTOR), but not which files went onto them. Forensic experts can sometimes piece together clues, never a full list. If you want that list next time, it has to be recorded at the time: during a session, Rashnova writes down every file copied to or from a USB drive, with the drive's name and serial, sealed so it cannot be removed quietly. [Read the full answer](./answers/check-if-usb-was-plugged-in.md).

### How do I check USB history in Windows 11?

Open Device Manager, choose View, then Show hidden devices: drives used before appear greyed out. For more detail, the registry key HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Enum\USBSTOR lists storage devices, often with a serial number. Both show that a drive was connected, not what was copied, and an administrator can clear them. Rashnova keeps each USB drive plugged in, when, and every file copied to it, in a sealed record on your computer. [Read the full answer](./answers/check-if-usb-was-plugged-in.md).

### What is the best free app to see what someone did on my computer?

Be careful: many "monitoring" apps are keyloggers or spyware that capture screens and typing, which is a privacy risk in itself and often illegal on someone else's device. For your own computer, Rashnova is built the other way round: it never records your screen, what you type or what is inside your files. It notes what happened (sign ins, USB drives, and during a session every file opened and program started), seals it so any change shows, keeps it on your computer, and reads it back in plain words. It is free for Windows 10 and 11. [Read the full answer](./answers/free-tools-see-what-happened-on-windows-pc.md).

### How do I prove a document was created on a certain date?

You can prove it existed by a date, which is usually what matters. Fingerprint the file (a SHA-256 hash) and have the fingerprint witnessed by someone you do not control: a time stamp authority (RFC 3161) or Bitcoin through OpenTimestamps. The file's own date is not proof; anyone can change it. [Rashnova Proof](https://www.alcyonesecure.com/proof) does it in one step, free and offline, with four independent witnesses and a certificate, and the file never leaves your computer. [Read the full answer](./answers/prove-a-file-existed-on-a-date.md).

### Is emailing a file to myself proof of the date?

It is weak proof. It rests on one email provider's records and on your account, the dates can be disputed, and it is hard for anyone else to check. A trusted time stamp over the file's fingerprint is stronger, because an independent party signs the time and anyone can check it later. Rashnova Proof gives you four independent witnesses for free, without the file leaving your computer. [Read the full answer](./answers/how-to-timestamp-a-file-for-free.md).

### How can I check if a PDF has been altered?

If it is digitally signed, open it in a PDF reader and look at the signature panel: it says whether the document changed after signing. If you have the original, compare fingerprints (Get-FileHash on Windows): one changed byte gives a different result. If it was proved, check it against its proof. Without a signature, an original or a proof, you usually cannot be sure, which is why proving important documents the day you receive or sign them is worth it. [Read the full answer](./answers/check-if-a-pdf-was-altered.md).

### How do I prove a photo is original and not edited?

Keep the original file from the camera or phone, not a forwarded copy, and prove it the same day: a proof shows those exact pixels existed by that time, so any later edit no longer matches. If the photo carries Content Credentials (C2PA), they record its source and edits. Rashnova Proof proves photos free and offline, and Origin reads a photo's credentials, facts and time stamps on your computer. No tool can promise a picture shows the truth. [Read the full answer](./answers/prove-photo-taken-before-a-date.md).

### Is a blockchain timestamp legally valid?

It can be evidence, but no timestamp is automatically accepted. Courts in some countries already accept hash checks and blockchain records; in the EU only qualified time stamps are presumed accurate; in India an electronic record usually comes with a certificate under Section 63 of the Bharatiya Sakshya Adhiniyam. A proof is stronger with several independent witnesses and an open way to check it. Rashnova Proof uses four, and fills a facts sheet a lawyer can use. This is not legal advice.

### What is the best free way to timestamp a file?

Use more than one independent witness, keep the file on your own computer, and make sure anyone can check the result without the company that made it. Doing that by hand takes a time stamp authority, OpenTimestamps and some command line work. Rashnova Proof does all of it in one drop, free, with four witnesses (drand, two time stamp authorities and Bitcoin), two signatures (one post quantum) and a certificate, checkable in any browser, offline. [Read the full answer](./answers/how-to-timestamp-a-file-for-free.md).

### Why should I install Rashnova?

Because the moments that matter happen when you are not looking: a repair, a lent laptop, a shared computer, a file you may need to prove one day. Rashnova keeps a sealed record of what happened on your computer and proves any file existed, exactly as it is. It is free, works offline, keeps everything on your computer, never records your screen, typing or files' contents, and nobody can quietly rewrite its record, not even us. [Download it free](https://www.alcyonesecure.com/download) for Windows 10 and 11.

## General

*What we make, who it is for, where to start*

### What is Alcyone Secure?

Alcyone Secure is a cybersecurity software company focused on protecting devices in real world situations. Our flagship is Rashnova, the evidence layer for Windows: it keeps a tamper evident record of what happens on your machine: every day, and especially when it leaves your control. We also ship CipherSuite (a workspace for security professionals), the Risk Awareness Platform, and a DPDP compliance service. See [the product catalogue](https://www.alcyonesecure.com/products).

### What does Rashnova mean?

Rashnova joins two words. **Rashnu** is the judge of souls in the Zoroastrian tradition of ancient Persia, called “the straightest”, whose golden scales favour no one: “as much as a hair’s breadth it will not turn”. **Nova** is a star that suddenly shines bright. Our company is named after Alcyone, the brightest star of the Pleiades, and Rashnova is the new light beside it. Together the name says what the product does: an honest record of what actually happened, whoever did it. [The whole story, with sources](https://www.alcyonesecure.com/about).

### How do you say Rashnova?

rash · NO · vuh. The stress is on the middle syllable, NO.

### Is Rashnova the product that used to be called Black Box?

Yes. It is the same recorder from the same team, with a new name and the same promises: the recorder is free forever, it records activity and never the content of your files, and nobody but you can read your logs. People still describe it as a black box for your laptop, which is a fair picture of what it does. Its name is Rashnova.

### Is Rashnova free?

Yes, the recorder is free, forever. Always on tamper evident recording, the Readout, Monitor Now, Repair Mode, Handover Mode, USB storage blocking, every USB device and every copy to one on record, Rashnova Proof, Origin, and at least 35 days of history all run on your device at no cost, with no card and no trial clock. Personal, coming soon at ₹199 a month or ₹1,999 a year (US$5.99 or US$59), will add a copy of your record off the computer, proofs' copies in the cloud, up to 10 years of history, three more themes and up to 3 computers. Full breakdown on [the pricing page](https://www.alcyonesecure.com/pricing).

### Is it safe to give my phone or laptop to a repair shop?

It carries a real, documented risk. A 2022 University of Guelph field study found technicians snooped on customer data in 6 of 16 repairs of a simple audio fault, and in 2021 Apple paid a confidential multimillion-dollar settlement after repair technicians leaked a customer’s private photos. See the full evidence on [the case files page](https://www.alcyonesecure.com/risks).

### Where can I download Rashnova?

From [the download page](https://www.alcyonesecure.com/download), free. You sign in with a free account to download, because the app sends us nothing and that is the only way we know how many people use it; the app itself never asks you to sign in. The installer brings everything Rashnova needs, including its own copy of Microsoft's .NET 10, so nothing else is downloaded during setup; recording works offline.

### Why does my browser or Windows warn me about the installer?

Because the installer is not code signed yet: we do not have a code signing certificate yet. Your browser may say the file isn't commonly downloaded, because each new version is a new file with no history yet: choose **Keep** in your browser's downloads. When you run it, Windows SmartScreen may warn about it, as it does about any unsigned installer; choose **More info**, then **Run anyway**. Before you do, you can check the file is the one we published: its SHA-256 is listed on [the download page](https://www.alcyonesecure.com/download). In PowerShell run `Get-FileHash "$env:USERPROFILE\Downloads\Rashnova-1.3.0.msi"` and compare the long value with the one on the page. They must match exactly.

## The recorder

*What it records, what it refuses to record, where it runs*

### Does Rashnova run all the time?

It can, once you switch it on. Continuous recording is off until you choose it; after that there is no session to remember to start. It runs as a quiet Windows service, survives reboots, and seals every event into the same hash chain. Repair Mode is the extra step on top: when the device is about to leave your hands, you arm it, and that window is watched closely and sealed into a report at the end. Everything remains a switch you control. If you would rather it did not run continuously, you can stop it, nothing here is forced on you.

### Is Rashnova spyware?

No: it is the opposite of spyware in every way that matters. Spyware hides from the device owner and reports to someone else. Rashnova runs visibly on your machine and records for you. The record stays on your device; the second copy is encrypted, and Rashnova opens it only after your PIN is checked. Ending a Repair session, exporting a report and deleting data all need your PIN. You own the data, the settings, and the exports. Nothing is collected behind your back, and nothing from your record leaves your device.

### What information does Rashnova record?

USB devices plugged in and removed, and every file copied to or from one; files opened, created, copied, moved, renamed and deleted during a session; programs started, and PowerShell scripts during a session; sign ins, failed sign ins, sign outs, starts, shutdowns and restarts; user accounts created or deleted; clock changes; changes to important Windows settings; anything done to Rashnova itself, and the health of its own record. Always on recording keeps only the serious things. It never records your screen, what you type, passwords, what your messages say, what is inside your files, the address or content of the pages you visit, or your camera or microphone. During a session, the title of a browser tab is recorded. A file's name is recorded, never what is in it. Everything stays on your computer.

### What is the Readout?

The Readout is a statement about your own machine, covering the last 7 days. In aviation, extracting and interpreting a recovered flight recorder's data is called the readout: this is the same thing for your computer. It opens with one honest verdict, usually “nothing unusual this week”, then leads with up to three things worth a look (the rest are one click away): a USB device you have never used before, an app reading a folder for the first time, a machine that started at 02:14 with nobody signing in. It is built on your machine from your own log, and nothing is uploaded to produce it.

### Can I turn the Readout off?

Yes. It is on by default because most people want it, but it is a switch like everything else, and you choose which day it arrives on. Turn it off and the recorder keeps running exactly as before: your log, your hash chain and your reports are unaffected. The same applies to always on recording. Rashnova is built so the owner decides what runs: start what you want, stop what you don't. A recorder you cannot control would just be surveillance with better branding, which is the opposite of the point.

### Can I tell the Readout when something was me?

Yes, and it is the most useful thing you can do with it. Every item the Readout raises carries two buttons: That was me, and That wasn't me. Marking something as yours stops it being raised again, so the Readout gets quieter and more accurate the longer you use it, the opposite of tools that grow noisier over time. Marking something as not yours takes you straight to the sealed evidence for that moment, which you can export. Those labels stay on your device. They are never uploaded and never used to build a profile of you.

### Can I trust the numbers in the Readout?

You can check them, which is better. Each Readout says whether the part of the record it summarises verified intact, so it is not just a rendered summary, it is a sealed statement you could hand to someone else. If the chain is broken anywhere in that window, the Readout marks itself unverified rather than presenting the counts as fact. And if part of the week is missing, it says so instead of quietly showing a smaller number.

### What is Monitor Now?

Monitor Now is a thirty second scan showing what is touching your files right now, which processes are reading and writing, which folders they are working in, and what is currently connected. It answers a specific question: something feels off, what is happening on this machine at this moment? It runs entirely on your device, needs no account, and uploads nothing. Its findings are recorded, but it is a live look rather than a sealed session. For evidence you intend to hand to someone else, use Repair Mode, which seals the whole window into a verifiable report.

### What is Repair Mode?

Repair Mode is the posture you arm before your device leaves your hands, at a repair counter, during a handover, any time someone else will be alone with the machine. While it is on, every file opened, copied, renamed or deleted, every program started and every USB device plugged in, with every file copied to it, is recorded, and everything from the moment you arm it until you disarm it is sealed into a single session. At the end you get a report with a verdict. USB storage blocking during Repair Mode arrives in an update soon. It is free, and it is the one moment where the recorder stops being a mirror and becomes a witness.

### Can Rashnova block USB drives?

Yes. From version 1.2, switch on USB storage blocking in Settings with your PIN, and memory sticks and external disks no longer open, fast USB 3 drives included. If someone switches USB storage back on outside Rashnova, that is recorded as tampering and it is blocked again within seconds. Like everything else it is a switch you control, off until you turn it on, and every USB device plugged in is still recorded, with its VID, PID and serial number.

### Does Rashnova record my device's location?

Not in this version. Rashnova records no location and makes no location lookups at all. Location recording comes in a later version, with the optional cloud backup, and will be off until you switch it on.

### Does Rashnova work offline?

Yes. Recording, the Readout and reports need no internet. Rashnova makes two small requests, neither carrying anything from your record: a daily check for a newer version, and a check of the time against Microsoft's time server during a Repair session.

### Does Rashnova work on Windows 10 and 11?

Yes. Rashnova supports Windows 10 (build 1903 and later) and all Windows 11 versions, both consumer and professional editions. Minimum requirements: 30 MB RAM, 50 MB disk.

### How much storage does Rashnova use?

Very little. The record is kept compressed on your computer, typically 5 to 50 MB depending on how much happens on the machine and how long history is kept.

### Does Rashnova capture what websites I visit?

No. It never records the address or the content of the pages you visit. During a Repair or Handover session it does record the title of a browser tab, and a private window is noted without its title.

### Does Rashnova log my passwords or what I type?

No. Rashnova does not capture keystrokes, clipboard contents, or screen pixels. It captures metadata about activity: which programs ran, which commands executed, which USB devices were inserted, which registry keys changed. It records metadata about activity, not the content of your life.

### What does Rashnova do with PowerShell commands?

It records PowerShell being started, and during a Repair or Handover session the commands and scripts that run, so a script someone ran while you were away is on the record. It records what was run, never what it printed. Rashnova turns on Windows' own PowerShell script logging only while a Repair or Handover session runs, and puts it back as it was when the session ends.

## Rashnova Proof & Origin

*Prove a file existed, exactly as it is, and see where a file came from. Free, on your computer*

### Is Rashnova Proof really free?

Yes. Making proofs, keeping them on your computer and checking them is free, forever. The witnesses that fix the time are free public services, so it costs us nothing to run, and we charge nothing for it. Only a copy of your proofs in the cloud, which comes with the paid plan, will cost money.

### Is my file uploaded anywhere?

No. The file is fingerprinted on your computer and never leaves it. When you are online, only a salted fingerprint goes to the public witnesses, never the file, and nothing goes to Alcyone.

### What does a proof prove, and what does it not?

It proves this exact file (one changed byte gives a different fingerprint), when it existed (the window of time witnessed by others), and that the proof was made on this Rashnova installation and has not been altered. It does not prove who made the file or who owns it, that what it says is true, or that a court will accept it.

### Who witnesses the time?

Four independent witnesses, never Alcyone. A public random value from the League of Entropy (drand) shows the proof was not made before a moment; two time stamp authorities, DigiCert and Sectigo, sign the time (RFC 3161); and OpenTimestamps puts the proof into a Bitcoin block, usually within a few hours. The computer's clock is also compared with India's official time (NPL).

### Can someone check my proof without Rashnova?

Yes. Every proof is one .rproof file that carries verify.html: open it in any browser, offline, and drop the file in. VERIFY.md gives the same checks with standard tools such as OpenSSL. The official checker is also published on this site with its own fingerprint. If Rashnova disappeared tomorrow, your proofs would still check.

### Why two signatures, and what is post quantum?

Every proof is signed twice: with a classic signature (ECDSA P-256, kept in your computer's security chip when it has one) and with a post quantum one (ML-DSA-65, the NIST standard FIPS 204). NIST plans to retire today's signatures between 2030 and 2035; the second signature is there so a proof made today still stands after that.

### Will a court accept a Rashnova proof?

Nobody honest can promise that, and we do not. A proof shows that this exact file existed by a certain time. For evidence forms, Rashnova fills a facts sheet with what your computer knows, for a lawyer or an expert to complete: India (Section 63 of the Bharatiya Sakshya Adhiniyam, 2023), the USA (a Federal Rule of Evidence 902(14) certification) and a general sheet. It is not legal advice.

### My photo does not match its proof. Why?

A photo resent by WhatsApp or email is recompressed, so it is no longer the same bytes, and it no longer matches. Prove the original file and keep it; check that same file later.

### What if my computer is offline?

The proof is made at once, and the public times are added the next time the computer is online.

### Can I prove a whole folder?

Yes. A whole folder becomes one proof, and one file can later be shown on its own without revealing the others.

### What is Origin?

Drop a file into Origin and Rashnova says where it came from, whether it changed, and when it existed. It reads what the file and its proofs say: Content Credentials (C2PA), photo facts, time stamps (RFC 3161), Bitcoin (OpenTimestamps) and Rashnova proofs.

### Is the file uploaded to check it?

No. Origin reads the file on your computer; nothing is uploaded. Bitcoin is asked only when you say so, and only for a block number.

### Can Origin tell me whether a picture is real?

Origin reports what the file and its proofs say, and says plainly when something cannot be relied on. It is not a verdict on whether a picture shows the truth.

## Privacy & the cloud

*Local first by default, and even the cloud can't read you*

### Can Alcyone employees read my logs?

No, and not as a promise, as an architecture. Your record is encrypted on your device, and the key never leaves it. When Personal arrives, what our servers hold will be ciphertext we cannot open. A breach of our own infrastructure would leak nothing readable. The website never displays log content for the same reason: there is nothing readable to display.

### Does Rashnova send my data to the cloud?

Not unless you turn it on. Today nothing from your record leaves your device at all: cloud backup is not in this version. When [Personal](https://www.alcyonesecure.com/pricing) arrives, encrypted copies of your logs will be mirrored to tamper evident cloud storage so they survive even if the device is wiped. Encryption happens on your machine before upload; the cloud only ever receives ciphertext.

### How do I get my logs back if my device is stolen or wiped?

Once Personal launches: request your logs from your account, the request has to come from the email you signed in with. We review each request by hand before releasing anything, then send your encrypted file to that address. It opens only in the Rashnova app, and only with your password. We never see the contents: what we hold is ciphertext we cannot open, so the manual review is a check on *who is asking*, never on what is inside. On the free tier the log lives only on the device, which is exactly the gap Personal exists to close. The flow is described on [the pricing page](https://www.alcyonesecure.com/pricing).

### Can I export my activity logs?

Yes. Reports and logs export from the app at any time, analyse them with your own tools, hand them to a forensic expert, or preserve them as evidence.

### Is my record encrypted?

Yes. During a Repair or Handover session, a second copy of your record is kept encrypted on your device, and it cannot be opened without your PIN on this machine. The record is also sealed, so it cannot be changed without that showing. The key never leaves your computer. We use well established, standard cryptography and nothing of our own invention.

## Tampering & evidence

*The PIN, the sealed record, and what happens when someone interferes*

### Can repair technicians disable Rashnova?

Not silently. A Repair session ends only with your PIN. Stopping the recorder needs administrator rights, and if it is stopped anyway, Windows starts it again within seconds, the session carries on, and the report shows the gap and how long it lasted.

### What happens if I forget my PIN?

It cannot be recovered: not by us, and not by signing in, because a way to recover it would be a way around it for anyone who has the computer. Starting a Repair session, exporting a report and deleting data need the PIN. Turning recording off never needs it, so a forgotten PIN can never keep you being recorded.

### How do hash chains work?

Each entry is sealed to the one before it. Edit or delete one entry and every entry after it stops matching; the break itself is the proof. Tamper evidence becomes a mathematical property of the file, not a policy that depends on anyone behaving.

### Can Rashnova prevent tampering?

It is built to make things provable rather than to stop them, with one real barrier: USB storage blocking, a switch in Settings. Its core job is evidence: a cryptographically verifiable record that tampering happened, when, and how. In most disputes, evidence beats prevention: you can't un copy a file, but you can prove it was copied.

### How is Rashnova different from antivirus?

Antivirus watches for malicious code. Rashnova watches for people. A technician who opens your photo folder, an intern copying the shared drive, a coworker at your unlocked desk: none of that triggers antivirus, because it's all done with legitimate access. Rashnova records it into a log that can't be quietly rewritten. Antivirus catches viruses; Rashnova catches people.

## Legal & compliance

*DPDP Act 2023, GDPR, and forensic logs in court*

### Is it legal to use Rashnova?

On your own device: yes. Recording activity on hardware you own is lawful in most places, and in India the DPDP Act 2023 does not apply to data an individual processes for personal or domestic purposes. Recording other people is different: tell everyone who uses the machine (the app itself reminds you to), and never use it to watch a partner, a family member or anyone without a lawful basis. Nothing leaves your computer, so Alcyone never receives your record. This is not legal advice; consult counsel for your situation.

### Does Rashnova help with DPDP Act 2023 compliance?

It provides one of the technical controls regulators expect from a serious data fiduciary: tamper evident records of who did what on a device. We unpack the practical work in the [DPDP guide for businesses](./blog/dpdp-act-2023-india-business-guide.md), and offer a full advisory service at [DPDP Compliance](https://www.alcyonesecure.com/products/dpdp).

### Can Rashnova logs be used as evidence in court?

They are built to be useful as evidence: captured at the moment of the event, sealed so any alteration shows, and exported with a fingerprint of the chain. In India, electronic records are admitted under Section 63 of the Bharatiya Sakshya Adhiniyam, 2023, which asks for a certificate describing the device and how the record was produced; a sealed report gives that certificate something concrete to point to. Admissibility is always decided by the court under the rules that apply to your case, but a tamper evident record is far stronger than a screenshot or a memory. This is not legal advice.

### Is monitoring an employee device with Rashnova legal?

It depends on your jurisdiction, what you tell employees, and whether the device is company owned. In India, an organisation that records staff activity is a data fiduciary under the DPDP Act 2023: it needs a lawful basis (the Act allows processing for employment purposes, including protecting the employer from loss or liability and keeping trade secrets confidential), a clear notice to the people affected, and reasonable security for the record. Written disclosure is the sensible baseline everywhere. We do not provide legal advice; consult a qualified lawyer before deploying monitoring in a workplace.

## Other products

*CipherSuite, Awareness, and the DPDP service*

### What is CipherSuite?

A free, live cybersecurity workspace for pentesters, bug-bounty hunters, SOC analysts, and security students: findings, evidence, notes, and AI assisted reports in one place. Read more at [/products/ciphersuite](https://www.alcyonesecure.com/products/ciphersuite).

### What is the Risk Awareness Platform?

AI powered security awareness training and DPDP compliance auditing for organisations, role based dashboards, scenario assessments, automated reports. Details at [/products/awareness](https://www.alcyonesecure.com/products/awareness).

### What is the DPDP Compliance service?

A technical advisory service for Indian businesses working toward DPDP Act 2023 compliance: assessment, gap analysis, and a documented remediation roadmap. NDA-first, vendor-neutral. Tiers and pricing at [/products/dpdp](https://www.alcyonesecure.com/products/dpdp).

### Do these products work together?

Yes, and each stands alone. Rashnova produces device level evidence. CipherSuite is the professional workflow on top of evidence. Awareness builds the human layer. The DPDP service ties it to the legal layer. No bundle lock in.

## Billing & support

*What we charge, how accounts work, how to reach us*

### Do I need an account to use Rashnova?

To download it, yes: a free account, so we know how many people use Rashnova (the app sends us nothing). The app itself runs without one and never asks you to sign in. The same account will carry Personal when it arrives: cloud backup, log retrieval, and multiple devices under one identity. Sign up at [/signup](https://www.alcyonesecure.com/signup).

### Can I protect multiple devices?

Yes. The free app works on each device without signing in. [Personal](https://www.alcyonesecure.com/pricing), coming soon, will cover multiple devices under one account. For team and fleet deployment, [talk to us](https://www.alcyonesecure.com/contact?topic=business).

### Can my company use the free version?

Yes, it can download and use it. The free version is made for individuals, so for organisations we also have Rashnova for Organisations: proofs issued in your organisation’s name and from its own email, deployment across your computers, organisation settings and a direct line to our team. On top of that we tailor it to you, for example mostly Proof, closer protection for particular files, or proofs for a specific kind of document. [Tell us what you need](https://www.alcyonesecure.com/contact?topic=business) and our team will call you or write back. See [Article 2 of the Terms](https://www.alcyonesecure.com/terms).

### What happens if I cancel Personal?

The recorder keeps working on your device, free, forever: cancellation never touches local protection, and Proof and Origin stay free too. If your plan ends, we keep your proofs' copies in the cloud for one month and email you. Continue the plan, or keep them on your computer from Rashnova with your password. After that month they are deleted. The proofs on your computer are not affected.

### Something is not working. What should I send?

Write to [support@alcyonesecure.com](mailto:support@alcyonesecure.com) with what you saw and your Windows version. If we need more, our team sends you a small support tool that reads only facts about your install, never your files or your record, and you see everything it gathers before you decide to send it.

### How do I contact support?

Use [the contact form](https://www.alcyonesecure.com/contact?topic=support), or email [support@alcyonesecure.com](mailto:support@alcyonesecure.com), for general help (24 hour response target). Security disclosures: [report a vulnerability privately on GitHub](https://github.com/sathvik-zoldyck/rashnova/security/advisories/new), or email [contact@alcyonesecure.com](mailto:contact@alcyonesecure.com). Privacy: [contact@alcyonesecure.com](mailto:contact@alcyonesecure.com). Sales: [contact@alcyonesecure.com](mailto:contact@alcyonesecure.com).

### Is there enterprise or volume pricing?

Yes: volume pricing, centralised deployment, dedicated support, and custom configuration for organisations. [Talk to us](https://www.alcyonesecure.com/contact?topic=business), or email [contact@alcyonesecure.com](mailto:contact@alcyonesecure.com).

---

*Source of record: [https://www.alcyonesecure.com/faq](https://www.alcyonesecure.com/faq). This copy is generated from the website; edit the website, not this file.*

