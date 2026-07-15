# DPDP Act 2023, explained for Indian businesses (and what auditors actually look for)

*Compliance · Apr 2026 · 9 min read*

> A practical, founder-friendly walkthrough of India Digital Personal Data Protection Act 2023: what changed, what auditors test for, and why audit trails are the easiest mistake to fix.

India Digital Personal Data Protection Act 2023, usually shortened to DPDP, is the country first horizontal data protection law. It applies to almost any business that handles personal data about Indian residents, regardless of where the business is incorporated. If you have customers, employees, or vendors in India, you are very likely a data fiduciary under the Act.

This is not a legal document; it is a working summary written for founders, ops leads, and IT teams who need to know what to do this quarter, not in two years.

## What changed in plain English

- Consent must be specific, informed, and easy to withdraw. The blanket Terms checkbox does not satisfy this any more.
- Purpose limitation is binding. You can only process personal data for the purpose you collected it for.
- Data principals get rights: access, correction, erasure, and grievance redressal. You need a process, not just a policy page.
- Significant data fiduciaries face additional obligations including DPO appointment and periodic audits.
- Penalties go up to INR 250 crore for the worst classes of violation.

## Where most teams fail the audit

### 1. Inventory drift

The legal team data inventory does not match what is actually being collected by product. Engineering ships a new event tracker, marketing imports a CRM, customer success enables session-replay, and the inventory does not get updated.

### 2. Vendor sprawl without DPAs

Every SaaS tool that touches personal data is a sub-processor. If you do not have data-processing agreements with each one, you cannot meet your downstream-controller obligations.

### 3. No grievance workflow

Users have a right to file grievances; you have a duty to acknowledge and resolve them. A generic support inbox is not enough if there is no SLA, no triage path, and no record of resolution.

### 4. Audit trail is performative, not forensic

Most teams have logs. Few have logs that would survive a hostile insider. If your logs can be edited or deleted by anyone with admin access, they are not an audit trail; they are a story. We unpack this in [forensic logging vs activity monitoring](./forensic-logging-vs-activity-monitoring.md).

## What forensic-grade logging buys you

DPDP does not, today, mandate cryptographic log integrity. But auditors evaluate the credibility of evidence you produce. A tamper-evident log, where each entry is hashed and chained, is more credible than a log that the operations team can edit on a whim. Read more in our [hash chains explainer](./hash-chains-explained-non-cryptographer.md).

## A 90-day implementation plan

1. **Days 1 to 14:** rebuild the data inventory from product surface area, not from policy text. Tag each field with purpose and retention.
2. **Days 15 to 30:** identify and contract every sub-processor. Use a template DPA. Replace tools that will not sign.
3. **Days 31 to 60:** implement consent and purpose tagging in the product. Build a grievance workflow with a real SLA and accountable owner.
4. **Days 61 to 90:** deploy tamper-evident logging on systems that touch personal data. Validate that the logs survive a simulated insider event.

**Q: Does DPDP apply to me if I am based outside India?**

If you process personal data of Indian residents in connection with offering goods or services to them, yes.

**Q: What are the immediate priorities for an SME?**

Inventory, DPA backlog, grievance workflow, and audit-trail integrity. In that order.

**Q: Are repair shops covered by DPDP?**

If they handle personal data on customer devices, then under most interpretations yes. The Kolkata 2025 case shows what happens when shop-side practices fall short. See [our case study](./kolkata-phone-repair-shop-private-video-leak-2025.md).

---

*Published on the [Alcyone Secure blog](https://www.alcyonesecure.com/blog/dpdp-act-2023-india-business-guide). This document mirrors public website content for open, offline, and machine reading.*
