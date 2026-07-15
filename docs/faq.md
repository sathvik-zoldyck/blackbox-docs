# Frequently Asked Questions

Direct answers to the questions people actually ask about Black Box and Alcyone Secure — is it spyware, can we read your logs, is it legal, what happens when your device is stolen. Mirrored from [the website's FAQ](https://www.alcyonesecure.com/faq).

**37 answers on file · 7 channels.**

## Contents

- [General](#general) — what we make, who it is for, where to start
- [The recorder](#blackbox) — what it records, what it refuses to record, where it runs
- [Privacy & the cloud](#privacy) — local-first by default — and even the cloud can't read you
- [Tampering & evidence](#security) — pin protection, hash chains, and what happens when someone interferes
- [Legal & compliance](#legal) — dpdp act 2023, gdpr, and forensic logs in court
- [Other products](#products) — ciphersuite, awareness, and the dpdp service
- [Billing & support](#support) — what we charge, how accounts work, how to reach us

<a id="general"></a>

## General

*What we make, who it is for, where to start.*

### What is Alcyone Secure?

Alcyone Secure is a cybersecurity software company focused on protecting devices in real-world situations. Our flagship is Black Box — a forensic flight recorder for Windows that creates tamper-evident records when your device leaves your control. We also ship CipherSuite (a workspace for security professionals), the Risk Awareness Platform, and a DPDP compliance service. See [the product catalogue](https://www.alcyonesecure.com/products).

### Is Black Box free?

Yes — the recorder is free, forever. Tamper-evident forensic recording, USB blocking, location recording, and in-app reports all run on your device at no cost, with no card and no trial clock. Premium (₹199 / $6 a month) adds the cloud layer: encrypted off-device backup, log retrieval, and multi-device support. Full breakdown on [the pricing page](https://www.alcyonesecure.com/pricing).

### Is it safe to give my phone or laptop to a repair shop?

It carries a real, documented risk. A 2022 University of Guelph field study found technicians snooped on customer data at 6 of 16 shops tested for a simple battery job, and in 2021 Apple paid a confidential multimillion-dollar settlement after repair technicians leaked a customer’s private photos. See the full evidence on [the case files page](https://www.alcyonesecure.com/risks).

### Where can I download Black Box?

From [the download page](https://www.alcyonesecure.com/download). The installer is small, digitally signed, and works fully offline. Free for individuals, Windows 10 and 11.

<a id="blackbox"></a>

## The recorder

*What it records, what it refuses to record, where it runs.*

### Is Black Box spyware?

No — it is the opposite of spyware in every way that matters. Spyware hides from the device owner and reports to someone else. Black Box runs visibly on your machine, records for you, stores its logs encrypted on your device, and can only be controlled with your PIN. You own the data, the settings, and the exports. Nothing is collected behind your back, and nothing leaves your device unencrypted.

### What information does Black Box record?

File access and modifications, process execution with full command lines, network connection attempts, USB device arrivals and removals (with VID, PID, serial), PowerShell script blocks, critical registry key changes (~18 high-value keys), browser window titles (not URLs or page content), and system configuration changes. It does not record keystrokes, clipboard contents, passwords, or screen pixels. All logs are encrypted and stored locally.

### Can Black Box block USB drives?

Yes. USB storage blocking is a free, built-in toggle: switch it on before a handover and USB storage devices simply will not work on your machine until you turn it off. Every connection attempt is still logged with the device’s VID, PID, and serial number — so a blocked exfiltration attempt becomes evidence too.

### Does Black Box record my device's location?

Only if you turn it on. Location recording is an optional toggle — useful when a device is out for repair or transit. Location entries go into the same encrypted, hash-chained log as everything else, on your device. Nobody but you can read them.

### Does Black Box work offline?

Yes. Black Box runs fully offline by default — monitoring, logging, and report generation need no internet. Only Premium cloud backup and update checks use a connection, and cloud sync resumes securely whenever a connection returns.

### Does Black Box work on Windows 10 and 11?

Yes. Black Box supports Windows 10 (build 1903 and later) and all Windows 11 versions, both consumer and professional editions. Minimum requirements: 30 MB RAM, 50 MB disk.

### How much storage does Black Box use?

The installer is around 3 MB. Activity logs are compressed and encrypted, typically 5 to 50 MB per device depending on activity volume and retention settings.

### Does Black Box capture what websites I visit?

It captures browser window titles, not URLs or page contents. A title like ‘HDFC NetBanking — Login’ is logged as high-risk activity for the audit trail; the actual URL and page content are never read or stored. Private/incognito windows log only that private browsing occurred, with no title content.

### Does Black Box log my passwords or what I type?

No. Black Box does not capture keystrokes, clipboard contents, or screen pixels. It captures metadata about activity: which programs ran, which commands executed, which USB devices were inserted, which registry keys changed. Not the content of what was typed or read.

### What does Black Box do with PowerShell commands?

It subscribes to Windows’ PowerShell logging provider and captures the script blocks that execute during a session. Internal housekeeping (tab completion, prompt rendering) is filtered out. Only actual command execution is logged, with a risk classifier flagging dangerous patterns such as encoded commands, download-and-execute chains, and Defender-tampering attempts.

<a id="privacy"></a>

## Privacy & the cloud

*Local-first by default — and even the cloud can't read you.*

### Can Alcyone employees read my logs?

No — and not as a promise, as an architecture. Logs are encrypted on your device, with a key derived from your credentials, before anything is stored or synced. What our servers hold on Premium is ciphertext we cannot open. A breach of our own infrastructure would leak nothing readable. The website never displays log content for the same reason: there is nothing readable to display.

### Does Black Box send my data to the cloud?

Not unless you turn it on. On the free tier, every log stays on your device — nothing is transmitted, ever. On [Premium](https://www.alcyonesecure.com/pricing), encrypted copies of your logs are mirrored to tamper-evident cloud storage so they survive even if the device is wiped. Encryption happens on your machine before upload; the cloud only ever receives ciphertext.

### How do I get my logs back if my device is stolen or wiped?

On Premium: request your logs from your account, and your encrypted file is sent to your registered email. It opens only in the Black Box app, only with your password — on any machine. On the free tier the log lives only on the device, which is exactly the gap Premium exists to close. The flow is described on [the pricing page](https://www.alcyonesecure.com/pricing).

### Can I export my activity logs?

Yes. Reports and logs export from the app at any time — analyse them with your own tools, hand them to a forensic expert, or preserve them as evidence.

### How does the encryption work?

AES-256-GCM authenticated encryption for log content, SHA-256 hash chains for tamper evidence, and PBKDF2 for key derivation from your PIN. Logs cannot be decrypted without your credentials, modified without detection, or silently deleted. The keys are derived on your device and never transmitted.

<a id="security"></a>

## Tampering & evidence

*PIN protection, hash chains, and what happens when someone interferes.*

### Can repair technicians disable Black Box?

Not silently. Black Box is protected by a PIN only you know, and the service is guarded by a watchdog: if any component is stopped unexpectedly, it restarts and the interruption itself is signed into the hash chain. A technician who tries to kill the recorder produces evidence of having tried.

### What happens if I forget my PIN?

Your PIN never leaves your device, and we cannot reset it for you — by design. During setup, Black Box gives you a 24-word recovery phrase; that phrase is the only way to regain access to your encrypted logs. Store it somewhere safe and offline. No email reset, support ticket, or anyone at Alcyone can decrypt your data — if that were possible, so could an attacker.

### How do hash chains work?

Each log entry contains a SHA-256 hash of the previous entry. Edit or delete one entry and every subsequent hash stops matching — the break itself is the proof. Tamper-evidence becomes a mathematical property of the file, not a policy that depends on anyone behaving.

### Can Black Box prevent tampering?

It prevents some (USB blocking stops storage devices from mounting at all) and makes the rest provable. Its core job is evidence: a cryptographically verifiable record that tampering happened, when, and how. In most disputes, evidence beats prevention — you can't un-copy a file, but you can prove it was copied.

### How is Black Box different from antivirus?

Antivirus watches for malicious code. Black Box watches for people. A technician who opens your photo folder, an intern copying the shared drive, a coworker at your unlocked desk — none of that triggers antivirus, because it's all done with legitimate access. Black Box records it into a log that can't be quietly rewritten. Antivirus catches viruses; Black Box catches people.

<a id="legal"></a>

## Legal & compliance

*DPDP Act 2023, GDPR, and forensic logs in court.*

### Is it legal to use Black Box?

On your own device: yes, in most jurisdictions — recording activity on hardware you own is generally lawful. Monitoring shared or workplace devices is regulated and varies by country; disclosure to users is the safer baseline everywhere. Black Box is built to align with the DPDP Act 2023 (India), GDPR (EU), and CCPA (USA). This is not legal advice; consult counsel for your situation.

### Does Black Box help with DPDP Act 2023 compliance?

It provides one of the technical controls regulators expect from a serious data fiduciary: tamper-evident records of who did what on a device. We unpack the practical work in the [DPDP guide for businesses](./blog/dpdp-act-2023-india-business-guide.md), and offer a full advisory service at [DPDP Compliance](https://www.alcyonesecure.com/products/dpdp).

### Can Black Box logs be used as evidence in court?

They are designed for it: original capture at event time, hash-chain integrity that makes alteration detectable, and a documented chain of custody. Admissibility always depends on jurisdiction and the rules of evidence in your case — but a tamper-evident log is categorically stronger than a screenshot or a memory.

### Is monitoring an employee device with Black Box legal?

It depends on your jurisdiction, the disclosures you make, and whether the device is company-owned. Clear written disclosure to employees is the safer baseline everywhere, and in India, GDPR-equivalent practice is the sensible bar. We do not provide legal advice; consult a qualified lawyer before deploying monitoring in a workplace.

<a id="products"></a>

## Other products

*CipherSuite, Awareness, and the DPDP service.*

### What is CipherSuite?

A free, live cybersecurity workspace for pentesters, bug-bounty hunters, SOC analysts, and security students — findings, evidence, notes, and AI-assisted reports in one place. Read more at [/products/ciphersuite](https://www.alcyonesecure.com/products/ciphersuite).

### What is the Risk Awareness Platform?

AI-powered security awareness training and DPDP compliance auditing for organisations — role-based dashboards, scenario assessments, automated reports. Details at [/products/awareness](https://www.alcyonesecure.com/products/awareness).

### What is the DPDP Compliance service?

A technical advisory service for Indian businesses working toward DPDP Act 2023 compliance — assessment, gap analysis, and a documented remediation roadmap. NDA-first, vendor-neutral. Tiers and pricing at [/products/dpdp](https://www.alcyonesecure.com/products/dpdp).

### Do these products work together?

Yes, and each stands alone. Black Box produces device-level evidence. CipherSuite is the professional workflow on top of evidence. Awareness builds the human layer. The DPDP service ties it to the legal layer. No bundle lock-in.

<a id="support"></a>

## Billing & support

*What we charge, how accounts work, how to reach us.*

### Do I need an account to use Black Box?

No — the free tier runs without an account. You create one only when you want Premium: cloud backup, log retrieval, and multiple devices under one identity. Sign up at [/signup](https://www.alcyonesecure.com/signup).

### Can I protect multiple devices?

Yes. The free tier is per-device with no account needed. [Premium](https://www.alcyonesecure.com/pricing) covers multiple devices under one account. For team and fleet deployment, email [contact@alcyonesecure.in](mailto:contact@alcyonesecure.in).

### What happens if I cancel Premium?

The recorder keeps working on your device, free, forever — cancellation never touches local protection. Your cloud copies are returned to you as an encrypted archive, then deleted from our servers after a 30-day grace window.

### How do I contact support?

Email [support@alcyonesecure.com](mailto:support@alcyonesecure.com) for general help (24-hour response target). Security disclosures: [security@alcyonesecure.com](mailto:security@alcyonesecure.com). Privacy: [privacy@alcyonesecure.com](mailto:privacy@alcyonesecure.com). Sales: [contact@alcyonesecure.in](mailto:contact@alcyonesecure.in).

### Is there enterprise or volume pricing?

Yes — volume pricing, centralised deployment, dedicated support, and custom configuration for organisations. Email [contact@alcyonesecure.in](mailto:contact@alcyonesecure.in) to discuss.

---

*Source of record: [alcyonesecure.com/faq](https://www.alcyonesecure.com/faq). Trust is good. Proof is better.*
