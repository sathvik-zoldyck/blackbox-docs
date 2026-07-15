# Insider wrongdoing at Tesla: how two former employees walked out with 100 gigabytes of confidential data

*Investigation · Apr 2026 · 9 min read*

> The 2023 Tesla insider breach exposed 75,735 employee records and showed how easily a departing employee can exfiltrate years of internal data without triggering a single alert. What happened, why endpoint security alone cannot catch it, and what session-level forensics would have shown.

**TL;DR** — Two former Tesla employees walked out of the company with approximately 100 gigabytes of confidential data — 23,000+ internal documents and personally identifying information of 75,735 current and former employees. Tesla discovered the breach only when a foreign newspaper notified them. Endpoint security treated the activity as authorised; without a session-level forensic record, there was no evidence trail until the data surfaced externally.

> **ARTICLE IN PRODUCTION** — We are finalising the long-form analysis, including the file-class breakdown, the offboarding-window timeline, and the session-record properties a recorder like Black Box would have surfaced. [Email us](mailto:support@alcyonesecure.com) if you would like an early draft for an internal insider-risk review.

Tesla's insider breach is one of the cleanest case studies in the limits of conventional endpoint security. The two individuals had legitimate credentials. They were inside the offboarding window. Standard data-loss-prevention rules treat that activity as authorised. No alerts fired.

Tesla learned about the exfiltration from Handelsblatt, the German publication that received the documents. By then the data had been in unauthorised hands for months.

## What was taken

Per Tesla's notification to the Maine Attorney General in August 2023, the breach included personally identifying information for 75,735 current and former employees, customer bank details, production secrets, and internal complaints about Full Self-Driving software. Total volume was reported at roughly 100 gigabytes across more than 23,000 internal documents.

## Why endpoint security missed it

Most endpoint DLP rules are tuned to surface anomaly: an unusual destination, an unusual time of day, an unusual file type. Insider exfiltration during the offboarding window does not look anomalous — the user is logging in from their normal device, on their normal hours, accessing files they have always had permission to read. The signal is in the volume and the intent, not the act.

## What a session-level forensic record would have shown

A hash-chained record of every file read, every USB device attached, and every network destination during the offboarding window would have produced two artefacts. First, an attributable timeline that survives any later denial. Second, a measurable spike — 100GB does not move silently when each event is committed to a tamper-evident chain. The detection window changes from months to the same business day.

The control is not preventative — a determined insider with legitimate access can still copy files. The control is evidentiary. Without it, the organisation has no answer to a regulator or a court when the question becomes, "what exactly left the building, when, and to where."

**Sources:**
- [Tesla data breach notification, Maine Attorney General (August 2023)](https://apps.web.maine.gov/online/aeviewer/ME/40/)
- [Handelsblatt original reporting](https://www.handelsblatt.com/)

---

*Published on the [Alcyone Secure blog](https://www.alcyonesecure.com/blog/tesla-insider-data-exfiltration-100gb-2023). This document mirrors public website content for open, offline, and machine reading.*
