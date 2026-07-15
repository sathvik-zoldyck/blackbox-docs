# The Marks & Spencer breach explained: how attackers used a third-party IT help desk to take down a £300M retailer

*Investigation · Apr 2026 · 11 min read*

> A detailed walkthrough of the April 2025 Marks & Spencer cyberattack — how social engineering against TCS help desk staff bypassed M&S's defences, and what tamper-evident session logging would have changed.

**TL;DR** — In April 2025, attackers socially engineered help desk staff at Marks & Spencer's outsourced IT provider, Tata Consultancy Services, into resetting passwords for legitimate-sounding employees. The breach disrupted M&S online operations for over six weeks, exposed 9.4 million customer records, and cost an estimated £300 million in operating profit. The breach surface was the trust boundary between client and contractor — exactly where forensic logging is least common.

> **ARTICLE IN PRODUCTION** — We are finalising the long-form analysis, including the call-script analysis, the TCS-side controls that failed, and the session-record properties that would have shortened detection. [Email us](mailto:support@alcyonesecure.com) if you would like an early draft for an enterprise threat-modelling exercise.

On 22 April 2025, Marks & Spencer's online order systems went dark. By the time forensic teams traced the entry point, attackers had already been inside for several days. The route in was not a zero-day. It was a phone call to a help desk run by a third-party IT contractor — and a successful impersonation of a legitimate M&S employee asking for a password reset.

This article walks through the publicly known timeline, the failure mode, and the kind of forensic record that would have changed the investigation. It draws on Reuters reporting, M&S statements, and testimony from the UK Parliament's Business and Trade Committee.

## What we know about the timeline

Marks & Spencer disclosed a cyber incident on 22 April 2025. Reuters and the Financial Times subsequently reported that attackers had social-engineered help desk staff at Tata Consultancy Services, M&S's outsourced IT service desk provider, into performing password resets for accounts that were not theirs. The threat actor has been publicly linked to the Scattered Spider cluster, which has used identical tradecraft against other large retailers.

## The structural failure

Outsourced help desk agents typically have privileged access to client identity systems but operate from machines and call-recording infrastructure run by the contractor. When a password reset is performed, the customer organisation has no independent record of who authorised it, what voice was on the call, or whether the agent followed identity-verification policy.

## What a tamper-evident session record would have changed

If every help desk session — including the call audio, the agent's screen, and the identity-verification steps — were captured into a hash-chained log readable by both the contractor and M&S, two things change. First, post-incident detection drops from days to hours, because each unauthorised reset can be replayed and audited. Second, the incentive structure on the agent side changes: a session that is permanently recorded and externally verifiable is materially harder to compromise through bribery or coercion.

The same primitive applies to every IT service-desk relationship, every outsourced support function, and every internal help desk that performs sensitive operations under time pressure.

**Sources:**
- [Reuters: M&S cyberattack details (April–October 2025)](https://www.reuters.com/)
- [UK Parliament Business and Trade Committee](https://committees.parliament.uk/)

---

*Published on the [Alcyone Secure blog](https://www.alcyonesecure.com/blog/marks-and-spencer-third-party-it-help-desk-breach-2025). This document mirrors public website content for open, offline, and machine reading.*
