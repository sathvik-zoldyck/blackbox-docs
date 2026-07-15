# About Alcyone Secure

> Security is not just prevention. **Security is accountability.**

Every serious security tool is built to stop attacks that arrive over the network. We build
for the moment none of them cover: when a device is physically in someone else's hands, and
the risk is a person, not a program. Alcyone Secure records the human layer of device
security — so that trust is never your only option.

This document mirrors the public [About page](https://www.alcyonesecure.com/about).

---

## The thesis

Anyone who has handed a laptop to a repair shop knows the feeling. The machine that holds your
photos, your money, your work goes behind a counter you can't see past. And every security
product you own has gone quiet, because none of them were built for this.

Black Box is our answer. Not prevention — a **witness**. A recorder that writes down what
happens to your device in a form nobody can quietly rewrite, encrypted so that nobody —
including us — can read it but you.

We are building it deliberately small and deliberately honest: local first, sealed before it
leaves the device, provable when it matters.

---

## What Black Box does

Black Box is a forensic flight recorder for Windows. It logs file access, process execution
(with command lines), network connection attempts, USB device arrivals and removals (with VID,
PID, and serial), PowerShell script blocks, critical registry changes, and browser window
titles — into an encrypted, tamper-evident **SHA-256 hash chain** stored on your device.

It does **not** record keystrokes, clipboard contents, passwords, or screen pixels. It captures
metadata about activity, not the content of what you type or read.

Full behaviour and limits are documented in the [FAQ](faq.md) and the
[field notes](blog/README.md).

---

## Why the recorder is free

Black Box version one is free for individuals, forever — and that was the plan from the start,
not a growth tactic. The company did not begin as a product idea. It began with research into
how personal data leaks from the devices people trust to strangers: repair benches, shared
workplaces, insider access. The recorder is the tool that research said was missing. Charging
individuals to defend themselves against it would have contradicted the entire reason for
building it.

The paid layer (Premium) exists for a narrow, honest reason: encrypted off-device backup and
log retrieval, so a wiped or stolen device does not take the evidence with it. The recorder
itself never sits behind a paywall.

---

## What we will never do

These are commitments, stated plainly:

- **Read your files.** Files opened by us: zero. Logs are encrypted on your device.
- **Hold a key that opens your logs.** Keys never leave your device — we could not comply with a
  demand to decrypt, because we physically can't.
- **Sell or share what the recorder sees.** Records sold: zero.
- **Put ads anywhere in the product.**
- **Phone home without being asked.** On the free tier, nothing is transmitted, ever.

If a number ever moves, you hear it from us first — publicly.

---

## The roadmap

The company log, kept the way the product keeps yours: append-only, each frame sealed, the next
one still on the runway.

- **2025 — Founded.** Alcyone Secure incorporated in India with one idea: devices need a witness,
  not another guard.
- **2026 · V1 — The recorder ships.** Local capture, SHA-256 hash chain, forensic reports. Free
  for individuals, forever.
- **2026 · V2 — The cloud layer.** *(In build.)* USB blocking, location recording, and encrypted
  off-device backup that survives a wiped machine.
- **Black Box Lite.** *(In development.)* The recorder goes mobile — a proper Android app, a mini
  Black Box for your phone that doubles as your authentication key for the desktop software.
  Lands with V2 or just behind it.
- **Next — Classified.** Announced when it ships. We don't hand our roadmap to our adversaries.

---

## Who builds it

Alcyone Secure was founded by **Sathvik R**. The credentials behind the product are on the
record, because the brand's whole premise is evidence over claims — don't claim it, file it:

- **Certificate in Data Protection Law** — Asian School of Cyber Laws, scored 100%. Taken before
  Black Box charged anyone a rupee, for one reason: if you build an evidence recorder, you should
  know first-hand what the law counts as evidence and what it calls protected.
  ([Verify](https://www.asianlaws.org/verify.php) · Cert № 1763720948-9193)
- **B.Tech, Computer Science** — the formal foundation under the practical work.
- **Offensive security** — self-taught, proven on real client engagements; CPTS path completed.
  You can't build a witness for attacks you've never run yourself. Hardware included.
- **Pre-founding research** — months inside the stolen-data trade before the company existed,
  tracking how drives leak from repair counters and where the files surface. That research is
  published in [the field notes](blog/README.md) and [the case files](risks.md).

---

## How it's funded

Until the paid cloud layer carries the company, development is funded by a separate **DPDP
compliance audit practice** — not by your data. The long-run model is the GitHub model:
enterprises fund the runway, individuals fly free.

---

## Contact

- General: support@alcyonesecure.com
- Security disclosures: security@alcyonesecure.com
- Privacy: privacy@alcyonesecure.com
- Sales / teams: contact@alcyonesecure.in

---

*Source of record: [alcyonesecure.com/about](https://www.alcyonesecure.com/about). Trust is good. Proof is better.*
