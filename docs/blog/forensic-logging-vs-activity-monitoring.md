# Forensic logging vs activity monitoring: what is actually admissible in court

*Engineering · Apr 2026 · 7 min read*

> Activity monitoring tells you what happened. Forensic logging produces evidence. The difference matters when it stops being a security question and starts being a legal one.

Most teams already have activity monitoring. So why is forensic logging a separate category? Because there is a sharp line between knowing what happened and being able to prove it to a third party who is willing to disagree with you.

## What activity monitoring is good at

Activity monitoring surfaces anomalies fast. Login from an unusual country, a process spawning a shell, a sudden spike in outbound traffic. The job is detection: get a human looking at the right thing within minutes. It is not built to be evidence. The data is normalised, enriched, and frequently re-written by the pipeline.

## What forensic logging adds

- Original capture: events recorded close to source, with the timestamps the operating system reported.
- Tamper evidence: each event hashed into a chain, so any later edit produces a detectable break (see [hash chains explained](./hash-chains-explained-non-cryptographer.md)).
- Chain of custody: the path from event to report is documented, deterministic, reproducible.

## What courts actually look for

- Authenticity: was the evidence produced by the system it claims to be from, and not altered since?
- Chain of custody: can the producer account for everyone who has touched it?
- System reliability: does the system produce consistent, reproducible output under normal operating conditions?

Activity monitoring almost never passes the first question without help. Forensic logging is designed to pass it standalone.

## When you actually need it

The moment a security incident becomes a legal matter. Insider data theft, employment disputes, regulator investigations, repair-shop incidents (see [our catalogue](./phone-laptop-repair-shop-privacy-breaches-real-incidents.md)), custody disputes over jointly used devices.

## What to look for in a forensic recorder

- Hash-chained or Merkle-anchored event log, not just append-only storage.
- Independent shadow copy, separately keyed.
- Local-first capture; events signed before any network transit.
- Documented, reproducible verification by any third party.
- Public threat model.

[Black Box](https://www.alcyonesecure.com/products/blackbox) meets these in its default install. The verifier is open, the chain is SHA-256, and the threat model is documented.

**Q: Does my EDR replace forensic logging?**

No. EDR is a security tool, forensic logging is a legal tool. They complement each other and a serious programme runs both.

**Q: Can a regular SIEM produce admissible evidence?**

Sometimes, with significant effort. The pipeline normalisation and re-writing typically used by SIEMs makes authentication harder. Forensic recorders are designed to skip that gap.

---

*Published on the [Alcyone Secure blog](https://www.alcyonesecure.com/blog/forensic-logging-vs-activity-monitoring). This document mirrors public website content for open, offline, and machine reading.*
