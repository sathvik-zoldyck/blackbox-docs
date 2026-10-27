> This page mirrors [The case files](https://www.alcyonesecure.com/risks) on alcyonesecure.com, the source of record.

# Can a repair shop steal your data? *It’s documented.*

**Yes, and not rarely.** In a 2022 University of Guelph field study, technicians at *6 of 16 repair shops* snooped on customer data on laptops left for a simple audio repair, and 2 of the 16 copied files off the device.

And the repair counter is only shelf one. The same exposure exists inside companies, the colleague at your unlocked desk, the day one intern on the shared drive, the contractor with a help desk login, the laptop that comes back wiped. Fourteen documented case files, on two shelves.

6 of 16

repair shops snooped on customer data in a 2022 University of Guelph field study: photos, browsing history, and documents.

[SOURCE: THE REGISTER, NOV 2022 ↗](https://www.theregister.com/2022/11/15/repair_technicians_data/)

2 of 16

shops copied customer files to external devices during the same study, one of them a file of passwords.

[SOURCE: HELP NET SECURITY, NOV 2022 ↗](https://www.helpnetsecurity.com/2022/11/16/computer-smartphone-repair-data-privacy/)

4 of 6

snooping technicians tried to cover their tracks, deleting Windows “Quick Access” traces, or browsing in ways that leave no log at all.

[SOURCE: SCHNEIER ON SECURITY, NOV 2022 ↗](https://www.schneier.com/blog/archives/2022/11/computer-repair-technicians-are-stealing-your-data.html)

$16.2M

average annual cost of insider incidents per organisation: colleagues, contractors, and departing employees with legitimate access.

SOURCE: PONEMON INSTITUTE, 2023

## The questions everyone asks, *answered on the record.*

Q.01, ON THE RECORD

### Can a computer repair shop steal your data?

Yes, and it is documented, not hypothetical. In a 2022 University of Guelph field study, technicians at 6 of 16 electronics repair shops accessed customers’ personal data without consent, and 2 of the 16 copied files off the device entirely.

The violations were not sophisticated attacks. Technicians opened photos, browsing history, and documents on machines left for a simple audio repair. Devices dropped off by women were snooped on more often, and the snooping specifically sought revealing photos and financial documents. Most shops had no privacy protocols at all: nothing stops a technician with your unlocked machine except their own restraint.

Q.02, ON THE RECORD

### Can a repair shop access your files without your password?

Yes. Your Windows password only protects the login screen, a technician can pull the drive and read it from another machine, or boot from a USB stick and bypass the login entirely.

If the disk is not encrypted, everything on it is readable without any credentials. Full disk encryption closes the offline path, but the moment a repair requires the machine unlocked and signed in, which most do, encryption no longer protects anything. A live, logged in session exposes your files, saved passwords, browser sessions, and cloud accounts to whoever is at the bench.

Q.03, ON THE RECORD

### Who watches the people who already have access?

Inside most organisations: nobody. Security tooling watches outsiders, a colleague at your unlocked desk, an intern copying the shared drive, or an admin reading beyond their task all look like normal, authorised work.

This is why insider incidents average $16.2M a year per organisation and take months to detect: every action is performed with a valid login. The intern downloading client lists is indistinguishable from the intern doing their job, unless there is a session level, tamper evident record of what was actually opened, copied, and connected. That record is what turns an unprovable suspicion into a closable case.

Q.04, ON THE RECORD

### How would you know if someone went through your files?

Without a dedicated recorder, you usually can’t. Windows keeps almost no user-readable trace of file access, and in the Guelph study, three of the six technicians who snooped cleared the few traces that exist, like the “Quick Access” recent files list.

This is the accountability gap the entire problem rests on: the incident leaves no fingerprint, so the victim never knows, so the behaviour never carries consequences. It is exactly what Rashnova exists to close: a tamper evident, hash chained log of every file opened, USB device inserted, and login during a Repair session. Deleting the log doesn’t work: every entry is cryptographically chained, so removal or alteration is itself detectable, and on Personal an encrypted copy already lives off device.

## Fourteen case files. *Open any of them.*

Every case is documented in public records or forensic case studies: repair counters, workplace machines, outsourced contractors, and insiders with legitimate access. None of them required a sophisticated attacker.

WHAT HAPPENED

Service technicians at major electronics chains have been documented opening customer photos, documents, and saved messages during routine repair. In several cases, files were copied to personal storage without consent.

WHY IT WORKS

When a device is powered on and unattended for hours, sensitive files are exposed. Without activity logging, the access leaves no trace, so the user cannot tell if anything happened.

SOURCES

FTC enforcement actions; consumer protection investigations into service centre conduct.

Repair technicians have been caught harvesting saved passwords, browser sessions, and payment tokens. Victims learned of the theft only when they noticed unfamiliar logins or fraudulent charges.

A logged in device is effectively unlocked. Anyone with sustained physical access can read browser stored credentials, walk away with auth cookies, and use them later from another network.

Consumer Reports; FBI Internet Crime Complaint Center (IC3) advisories.

Some technicians have installed remote access tools, keyloggers, or surveillance agents on customer devices. The malware persists after the device is returned, often surviving Windows reinstall if firmware level.

A repair shop bench is fully outside the customer's trust boundary. Installing software takes under a minute. Standard antivirus rarely flags signed remote management tools.

SANS Institute incident reports; published forensic case studies.

Technicians reset passwords and silently created new administrator accounts during repair. Devices appeared to function normally on return; the unauthorised access was discovered weeks later.

Password resets are routine troubleshooting. Without a verified record of what was changed, the user has no way to confirm the device is in the same security state it left in.

Consumer cybersecurity advisories; forensic findings from unauthorised account access cases.

Technicians reset device clocks and deleted Windows event logs to hide unauthorised access. Forensic teams later found gaps in event logs corresponding to the service window.

If the system clock is under the attacker, ordinary timestamps are worthless. Tamper evident logging anchored to external time sources is the only defence: an alteration shows up as a chain break.

Digital forensics literature; incident response case studies.

Workplace investigations regularly surface cases where a coworker used someone else’s unattended, logged in computer, reading private email, browsing HR and salary documents, or sending messages that appeared to come from the victim. The act takes minutes and is usually discovered only when its consequences surface.

On a shared floor, your unlocked session is your identity. Anything done on it is attributed to you by default, and without a per session activity record, you cannot prove that what happened at 3:41 PM wasn’t you.

SHRM workplace investigation guidance; corporate HR and disciplinary case records.

New joiners and interns are routinely granted broad access on day one: shared drives, client records, credentials. Insider risk reports document fresh hires copying company files to personal cloud accounts and USB drives within their first weeks: sometimes for a competitor, sometimes simply before quitting.

Onboarding grants access faster than trust is earned. Monitoring treats a valid login as a valid action, so a new hire copying the client list looks identical to a new hire doing their job. Insider incidents cost organisations an average of $16.2M a year and take months to detect.

Ponemon Institute, 2023 Cost of Insider Risks Global Report; Verizon DBIR insider-misuse findings.

Internal IT staff have used external drives to copy entire device contents during scheduled maintenance. Customer records and proprietary files left the building inside a pocket.

Bulk copy operations transfer terabytes in minutes. Standard monitoring usually does not flag a fast copy to a USB drive. Without a record of it, the event is invisible.

Enterprise breach disclosures; ISO 27001 audit findings.

Internal admins with legitimate access reached into employee personal files and email well outside the scope of an approved task. Users only learned of it months later.

Authorised access is not a defence against unauthorised use of that access. Without a session level activity record, the line between maintenance and surveillance is invisible to both parties.

SHRM workplace investigations; corporate IT audit reports.

Outsourced repair contractors hired staff with criminal records or zero security training and gave them unsupervised access to client devices. The resulting data theft had no audit trail.

When an organisation cannot answer who handled the device, when, and what they did, a regulator cannot accept any compliance claim. The accountability gap itself becomes the violation.

HIPAA breach notifications; PCI-DSS post-incident assessments.

An employee resigns, and the company laptop comes back factory reset: file activity, USB events, browsing history, all gone. Whatever was copied out in the final weeks is now unprovable. Legal teams call it spoliation; in practice it usually just ends the investigation.

If the device is the only place the record lives, whoever holds the device controls the evidence. A wipe destroys the local log by design. Only an off device, tamper evident copy, written while the events happened, survives the reset.

Digital forensics and legal hold case literature; incident response postmortems.

In April 2025, attackers gained access to UK retailer Marks & Spencer's systems by socially engineering employees at its third party IT service desk provider. Hackers impersonated legitimate staff over the phone and convinced help desk agents to reset passwords, giving attackers access to internal systems. The breach disrupted M&S online operations for over six weeks, exposed records belonging to roughly 9.4 million customers, and caused an estimated £300 million in operating profit damage. M&S subsequently ended its IT service desk contract with the contractor.

Help desk agents at outsourced IT vendors typically have privileged access to client systems but minimal forensic logging on their own activity. When an attacker successfully impersonates a legitimate employee, there is no tamper evident record showing who authorised the password reset, when, and on whose authority. The breach surface is the trust boundary between client and contractor, not the technical perimeter.

Reuters reporting; UK Parliament Business and Trade Committee testimony; M&S public statements (April-October 2025).

In May 2023, two former Tesla employees exfiltrated approximately 100 gigabytes of confidential data: over 23,000 internal documents, including personally identifying information of 75,735 current and former employees, customer bank details, production secrets, and internal complaints about Tesla's Full Self-Driving software. The data was shared with a foreign news organisation. Tesla discovered the breach only when notified by the recipient publication; the company's own systems had not flagged the exfiltration.

Employees with legitimate access can copy large volumes of data to personal devices in the period between resignation and offboarding. Standard endpoint security treats their activity as authorised. Without a session level forensic record of what was copied, when, and to which device, organisations have no evidence trail until the data surfaces externally.

Tesla data breach notification filed with Maine Attorney General, August 2023; Handelsblatt reporting; TechCrunch coverage.

In May 2025, cryptocurrency exchange Coinbase confirmed that personal data belonging to less than one percent of its users had been exposed after attackers bribed external customer support agents to share sensitive customer details, including names, account information, and partial Social Security numbers. The attackers attempted to extort a $20 million ransom; Coinbase refused, terminated the involved agents, and offered a matching $20 million reward for information leading to the perpetrators.

External support agents typically operate from machines outside the enterprise's direct visibility. When privileged access is exercised through an outsourced channel, the customer organisation cannot independently audit every action taken on its data. A forensic record of every customer record query, bound to the device, session, and time it occurred on: would have shortened detection from weeks to hours.

Coinbase public disclosure, May 2025; CEO Brian Armstrong public statements; SEC material disclosure filings.

## What should you do before *handing in a laptop?*

**Five steps, in order.** Short on purpose, a checklist people actually finish beats a longer one they skim. Each step shrinks the window in which someone can act on your data without leaving evidence. The last one is the only step that produces proof.
- **01 · Back up first** (verified). Make a verified backup of every important file before the device leaves your hands. If anything is altered, you have a baseline.

Make a verified backup of every important file before the device leaves your hands. If anything is altered, you have a baseline.
- **02 · Sign out of cloud accounts** (signed out). Sign out of cloud services and remove external drives. Every saved session is a credential exposure during repair.

Sign out of cloud services and remove external drives. Every saved session is a credential exposure during repair.
- **03 · Document the device state** (photographed). Photograph the home screen, installed apps, key settings, and the serial number. Anything that changes will stand out.

Photograph the home screen, installed apps, key settings, and the serial number. Anything that changes will stand out.
- **04 · Ask for a work record** (requested). Request a written summary of the work performed. It is not forensic evidence, but it forces the technician to commit to a story.

Request a written summary of the work performed. It is not forensic evidence, but it forces the technician to commit to a story.
- **05 · Run a forensic recorder** (armed). Install Rashnova before handover. It produces tamper evident proof of every USB connection, file open, login, and system event during the repair window.

Install Rashnova before handover. It produces tamper evident proof of every USB connection, file open, login, and system event during the repair window.

Also sensible, though not part of the procedure: use an authorised service centre where you have the choice, and keep your own note of when and where each device was serviced. Neither produces evidence, so neither earns a line on the checklist.

## What if your data *was already stolen?*

**Move fast and in this order.** The window between theft and misuse is where the damage is decided, most victims find out from a fraudulent charge, not from the shop.

MEMORY ITEMS · DO THESE FIRST, WITHOUT LOOKING ANYTHING UP
- **01 · Change every password, from a different device** (T+0). Start with email and banking. Assume saved browser passwords are burned. Do not do this from the returned machine until it is verified clean.

Start with email and banking. Assume saved browser passwords are burned. Do not do this from the returned machine until it is verified clean.
- **02 · Kill active sessions and tokens** (T+0). In Google, Microsoft, and banking accounts, sign out all devices and revoke app sessions. Stolen cookies keep working long after a password change if sessions stay alive.

In Google, Microsoft, and banking accounts, sign out all devices and revoke app sessions. Stolen cookies keep working long after a password change if sessions stay alive.

THEN, IN ORDER
- **03 · Watch the money** (T+1 HR). Alert your bank, watch card statements and credit activity. Fraudulent charges and new account fraud are the most common ways victims first find out.

Alert your bank, watch card statements and credit activity. Fraudulent charges and new account fraud are the most common ways victims first find out.
- **04 · Report it** (T+24 HR). File with the FTC (reportfraud.ftc.gov) or IC3 (ic3.gov) in the US, cybercrime.gov.in in India, or your local cybercrime unit. Reports create the paper trail later claims depend on.

File with the FTC (reportfraud.ftc.gov) or IC3 (ic3.gov) in the US, cybercrime.gov.in in India, or your local cybercrime unit. Reports create the paper trail later claims depend on.
- ONGOING05Preserve what evidence existsKeep the repair receipt, names, dates, screenshots of anything unusual. If you were running Rashnova, export the forensic report: that is exactly the evidence these cases usually lack.

Keep the repair receipt, names, dates, screenshots of anything unusual. If you were running Rashnova, export the forensic report: that is exactly the evidence these cases usually lack.

Every step above is damage control. *Recording the handover is prevention.*

FOR ORGANISATIONS

## Shelf B is your threat model. *Every seat, recorded.*

Nine of these fourteen cases happened inside organisations, with valid logins, on managed machines. Rashnova gives each device a tamper evident session record, so a colleague, contractor, or departing employee can no longer act without leaving evidence. Deployed across teams, with custom configuration.

## Short answers, *for the road.*

### Is it safe to give your laptop to a repair shop?

It carries a real, documented privacy risk. In a 2022 University of Guelph field study, technicians snooped on personal data at 6 of 16 shops. You can reduce the risk substantially: back up, sign out of accounts, encrypt the disk, and run a forensic recorder like Rashnova so any access during the repair window is provable.

### Do repair technicians go through your files?

Some do. The Guelph study documented technicians browsing photos, documents, and browsing history during unrelated repairs: and devices dropped off by women were targeted more often. Most shops have no privacy protocol preventing it.

### Can a repair shop access my data without my password?

Yes. An unencrypted drive can be removed and read from another machine, or the login can be bypassed by booting external tools. Full disk encryption stops offline reading, but a repair done on an unlocked, logged in machine exposes everything anyway.

### How can I prove someone accessed my files?

After the fact, you usually can't. Windows keeps few traces a user can see, and snooping technicians delete them. Proof requires recording during the exposure window: during a Repair session, Rashnova logs every file opened, USB device, and login into a tamper evident hash chain, so you get a verifiable record instead of a suspicion.

### How do companies prove what an employee did on a company laptop?

With session level, tamper evident recording. Standard monitoring treats a valid login as valid behaviour, so insider actions look like normal work. During a Repair session, Rashnova records file access, USB transfers, and logins into a hash chained log bound to the session: evidence that holds even when the actor had legitimate access.

### What if an employee wipes the laptop before returning it?

A factory reset destroys the local record, which is why the record can't only live on the device. With Rashnova Personal (coming soon), an encrypted, tamper evident copy of the log exists off device, so the wipe destroys nothing.

### What should I do before handing in my computer for repair?

Back up your data, sign out of cloud and banking sessions, remove saved payment methods where practical, enable disk encryption, photograph the device state, and start a Rashnova session so the entire repair window is recorded.

### What should I do if a repair shop stole my data?

Change every password from a different device, revoke active sessions, alert your bank, report to the FTC/IC3 (or cybercrime.gov.in in India), and preserve all evidence: receipts, names, dates, and any forensic logs from the repair window.

TRUST IS GOOD. PROOF IS BETTER.

## Stop guessing. *Start recording.*

Every case in this archive has the same missing piece: a record. Rashnova signs every file access, USB device, and login into a tamper evident chain during the exposure window: free, forever, on your device.

---

*Source of record: [alcyonesecure.com/risks](https://www.alcyonesecure.com/risks).*
