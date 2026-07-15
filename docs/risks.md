# Can a Repair Shop Steal Your Data? It's Documented.

**Yes — and not rarely.** In a 2022 University of Guelph field study, technicians at **6 of 16
repair shops** snooped on customer data left for a simple battery fix — and 2 of the 16 copied
files off the device.

And the repair counter is only shelf one. The same exposure exists inside companies — the
colleague at your unlocked desk, the day-one intern on the shared drive, the contractor with a
help-desk login, the laptop that comes back wiped. Fourteen documented case files, on two
shelves. *We name structures, not storefronts.*

This document mirrors the public [case files page](https://www.alcyonesecure.com/risks).
14 cases · cited sources · updated 2026.

---

## Direct answers

### Can a computer repair shop steal your data?

Yes — and it is documented, not hypothetical. In a 2022 University of Guelph field study,
technicians at 6 of 16 electronics repair shops accessed customers' personal data without
consent, and 2 of the 16 copied files off the device entirely. The violations were not
sophisticated attacks: technicians opened photos, browsing history, and documents on machines
left for a simple battery repair. Devices dropped off by women were snooped on more often, and
the snooping specifically sought revealing photos and financial documents. Most shops had no
privacy protocols at all — nothing stops a technician with your unlocked machine except their
own restraint.

### Can a repair shop access your files without your password?

Yes. Your Windows password only protects the login screen — a technician can pull the drive and
read it from another machine, or boot from a USB stick and bypass the login entirely. If the
disk is not encrypted, everything on it is readable without any credentials. Full-disk
encryption (BitLocker, FileVault) closes the offline path — but the moment a repair requires the
machine unlocked and signed in, which most do, encryption no longer protects anything.

### Who watches the people who already have access?

Inside most organisations: nobody. Security tooling watches outsiders. A colleague at your
unlocked desk, an intern copying the shared drive, or an admin reading beyond their task all
look like normal, authorised work. This is why insider incidents average $16.2M a year per
organisation and take months to detect: every action is performed with a valid login. That
record — of what was actually opened, copied, and connected — is what turns an unprovable
suspicion into a closable case.

### How would you know if someone went through your files?

Without a dedicated recorder, you usually can't. Windows keeps almost no user-readable trace of
file access — and in the Guelph study, technicians who snooped deleted the few traces that
exist, like the "Quick Access" recent-files list. This is the accountability gap the entire
problem rests on: the incident leaves no fingerprint, so the victim never knows, so the
behaviour never carries consequences. It is exactly what Black Box exists to close.

---

## Shelf A — The repair counter

Consumer devices in third-party custody.

### 01 · Unauthorized file access at retail service centres *(Consumer, ongoing)*
**What:** Service technicians at major electronics chains have been documented opening customer
photos, documents, and saved messages during routine repair. In several cases, files were copied
to personal storage without consent.
**Why it works:** When a device is powered on and unattended for hours, sensitive files are
exposed. Without activity logging, the access leaves no trace.
**Source:** FTC enforcement actions; consumer protection investigations into service-centre conduct.

### 02 · Credential theft during in-store device service *(Consumer, ongoing)*
**What:** Repair technicians have been caught harvesting saved passwords, browser sessions, and
payment tokens. Victims learned of the theft only when they noticed unfamiliar logins or
fraudulent charges.
**Why it works:** A logged-in device is effectively unlocked. Anyone with sustained physical
access can read browser-stored credentials and walk away with auth cookies.
**Source:** Consumer Reports; FBI Internet Crime Complaint Center (IC3) advisories.

### 03 · Backdoor installation during routine repair *(Consumer, ongoing)*
**What:** Some technicians have installed remote-access tools, keyloggers, or surveillance agents
on customer devices. The malware persists after return, often surviving a Windows reinstall if
firmware-level.
**Why it works:** A repair-shop bench is fully outside the customer trust boundary. Installing
software takes under a minute, and standard antivirus rarely flags signed remote-management tools.
**Source:** SANS Institute incident reports; published forensic case studies.

### 04 · Backdoor accounts created during repair *(Consumer, ongoing)*
**What:** Technicians reset passwords and silently created new administrator accounts during
repair. Devices appeared to function normally on return; the unauthorised access was discovered
weeks later.
**Why it works:** Password resets are routine troubleshooting. Without a verified record of what
was changed, the user has no way to confirm the device is in the same security state it left in.
**Source:** Consumer cybersecurity advisories; forensic findings from unauthorised-account-access cases.

### 05 · Clock manipulation and log deletion *(Consumer, ongoing)*
**What:** Technicians reset device clocks and deleted Windows event logs to hide unauthorised
access. Forensic teams later found gaps corresponding to the service window.
**Why it works:** If the system clock is under the attacker, ordinary timestamps are worthless.
Tamper-evident logging anchored to external time sources is the only defence — an alteration
shows up as a chain break.
**Source:** Digital forensics literature; incident-response case studies.

---

## Shelf B — Inside the building

Workplace, enterprise, and insider exposure.

### 06 · A colleague uses your unlocked machine *(Workplace, ongoing)*
**What:** Workplace investigations regularly surface cases where a coworker used someone else's
unattended, logged-in computer — reading private email, browsing HR and salary documents, or
sending messages that appeared to come from the victim.
**Why it works:** On a shared floor, your unlocked session is your identity. Without a per-session
activity record, you cannot prove that what happened at 3:41 PM wasn't you.
**Source:** SHRM workplace-investigation guidance; corporate HR and disciplinary case records.

### 07 · The intern with access to everything *(Workplace, ongoing)*
**What:** New joiners are routinely granted broad access on day one. Insider-risk reports document
fresh hires copying company files to personal cloud accounts and USB drives within their first
weeks — sometimes for a competitor, sometimes simply before quitting.
**Why it works:** Onboarding grants access faster than trust is earned. A new hire copying the
client list looks identical to one doing their job. Insider incidents cost organisations an
average of $16.2M a year and take months to detect.
**Source:** Ponemon Institute, 2023 Cost of Insider Risks Global Report; Verizon DBIR insider-misuse findings.

### 08 · USB bulk copying inside enterprise IT *(Enterprise, ongoing)*
**What:** Internal IT staff have used external drives to copy entire device contents during
scheduled maintenance. Customer records and proprietary files left the building inside a pocket.
**Why it works:** Bulk-copy operations transfer terabytes in minutes. Standard endpoint monitoring
usually does not flag fast disk-to-USB transfers at the kernel level.
**Source:** Enterprise breach disclosures; ISO 27001 audit findings.

### 09 · Sysadmin scope creep during maintenance *(Enterprise, ongoing)*
**What:** Internal admins with legitimate access reached into employee personal files and email
well outside the scope of an approved task. Users only learned of it months later.
**Why it works:** Authorised access is not a defence against unauthorised use of that access.
Without a session-level record, the line between maintenance and surveillance is invisible.
**Source:** SHRM workplace investigations; corporate IT audit reports.

### 10 · Inadequate vetting of third-party repair vendors *(Enterprise, ongoing)*
**What:** Outsourced repair contractors hired staff with criminal records or zero security
training and gave them unsupervised access to client devices. The resulting data theft had no
audit trail.
**Why it works:** When an organisation cannot answer who handled the device, when, and what they
did, a regulator cannot accept any compliance claim. The accountability gap itself becomes the
violation.
**Source:** HIPAA breach notifications; PCI-DSS post-incident assessments.

### 11 · The laptop comes back wiped *(Workplace, ongoing)*
**What:** An employee resigns, and the company laptop comes back factory-reset — file activity,
USB events, browsing history, all gone. Whatever was copied out in the final weeks is now
unprovable.
**Why it works:** If the device is the only place the record lives, whoever holds the device
controls the evidence. Only an off-device, tamper-evident copy — written while the events
happened — survives the reset.
**Source:** Digital-forensics and legal-hold case literature; incident-response postmortems.

### 12 · Third-party IT contractor compromise at a retail giant *(Enterprise, 2025)*
**What:** In April 2025, attackers accessed UK retailer Marks & Spencer's systems by socially
engineering employees at its third-party IT service desk provider — impersonating staff over the
phone to get passwords reset. The breach disrupted online operations for over six weeks, exposed
records of roughly 9.4 million customers, and caused an estimated £300 million in operating-profit
damage. M&S subsequently ended the contract.
**Why it works:** Help desk agents at outsourced IT vendors have privileged access but minimal
forensic logging on their own activity. There was no tamper-evident record showing who authorised
the reset, when, and on whose authority.
**Source:** Reuters; UK Parliament Business and Trade Committee testimony; M&S public statements (Apr–Oct 2025).
Full write-up: [the Marks & Spencer breach](blog/marks-and-spencer-third-party-it-help-desk-breach-2025.md).

### 13 · Mass exfiltration by departing employees *(Insider, 2023)*
**What:** In May 2023, two former Tesla employees exfiltrated ~100 GB of confidential data — over
23,000 internal documents, including PII of 75,735 current and former employees. Tesla discovered
the breach only when notified by the recipient publication; its own systems had not flagged it.
**Why it works:** Employees with legitimate access can copy large volumes to personal devices
between resignation and offboarding. Standard endpoint security treats their activity as
authorised.
**Source:** Tesla breach notification, Maine AG, Aug 2023; Handelsblatt; TechCrunch.
Full write-up: [insider wrongdoing at Tesla](blog/tesla-insider-data-exfiltration-100gb-2023.md).

### 14 · Bribed support agents exfiltrate customer records *(Insider, 2025)*
**What:** In May 2025, Coinbase confirmed that data belonging to under 1% of users was exposed
after attackers bribed external customer-support agents. The attackers attempted a $20M ransom;
Coinbase refused and terminated the agents.
**Why it works:** External support agents operate from machines outside the enterprise's direct
visibility. A forensic record of every customer-record query — bound to the device, session, and
time — would have shortened detection from weeks to hours.
**Source:** Coinbase public disclosure, May 2025; CEO statements; SEC material disclosure filings.

---

## Before you hand over a device

1. **Back up first.** A verified backup of every important file gives you a baseline if anything is altered.
2. **Sign out of cloud accounts.** And remove external drives. Every saved session is a credential exposure.
3. **Turn on disk encryption.** BitLocker or FileVault stops cold-boot and drive-removal extraction (not a live unlocked session).
4. **Document the device state.** Photograph the home screen, installed apps, and key settings — anything that changes will stand out.
5. **Use authorised channels.** Vetted service centres where possible. Screening is imperfect but better than a random storefront.
6. **Ask for a work record.** A written summary forces the technician to commit to a story.
7. **Track your repair history.** When, where, and why each device was serviced — a starting point if something surfaces later.
8. **Run a forensic recorder.** Install [Black Box](https://www.alcyonesecure.com/download) before handover — tamper-evident proof of every USB connection, file open, login, and system event during the repair window.

Full walkthrough: [the 2026 pre-repair checklist](blog/windows-laptop-pre-repair-checklist.md).

## If you think you've been breached

1. **Change every password — from a different device.** Start with email and banking. Assume saved browser passwords are burned.
2. **Kill active sessions and tokens.** Sign out all devices and revoke app sessions. Stolen cookies outlive a password change.
3. **Watch the money.** Alert your bank; watch card statements and credit activity.
4. **Report it.** FTC (reportfraud.ftc.gov) or IC3 (ic3.gov) in the US, cybercrime.gov.in in India, or your local cybercrime unit.
5. **Preserve what evidence exists.** Receipts, names, dates, screenshots. If you were running Black Box, export the forensic report.

---

## FAQ

**Is it safe to give your laptop to a repair shop?**
It carries a real, documented privacy risk. In the 2022 Guelph study, technicians snooped at 6 of
16 shops. You can reduce the risk substantially: back up, sign out, encrypt the disk, and run a
forensic recorder so any access during the repair window is provable.

**Do repair technicians go through your files?**
Some do. The Guelph study documented technicians browsing photos, documents, and history during
unrelated repairs — and devices dropped off by women were targeted more often.

**Can a repair shop access my data without my password?**
Yes. An unencrypted drive can be removed and read elsewhere, or the login bypassed by booting
external tools. A repair on an unlocked, logged-in machine exposes everything anyway.

**How can I prove someone accessed my files?**
After the fact, you usually can't — Windows keeps few user-visible traces and snooping technicians
delete them. Proof requires recording during the exposure window into a tamper-evident hash chain.

**What if an employee wipes the laptop before returning it?**
A factory reset destroys the local record — which is why it can't only live on the device. With
off-device, tamper-evident backup, the wipe destroys nothing.

---

*Source of record: [alcyonesecure.com/risks](https://www.alcyonesecure.com/risks). Trust is good. Proof is better.*
