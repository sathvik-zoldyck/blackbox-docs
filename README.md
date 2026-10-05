# Rashnova by Alcyone Secure: public documentation

> **Languages** · **English** · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Rashnova is the evidence layer for Windows**: a free app that keeps a sealed, tamper evident
record of what people and programs did on your PC, so you can check afterwards what happened while
someone else had it. At a repair shop, an IT desk, on a shared family computer, or lent to a
friend, Rashnova records the USB drives plugged in, the files opened and copied, the programs
started and the sign ins, and seals every entry to the one before it, so any change shows. Made by
[Alcyone Secure](https://www.alcyonesecure.com) for Windows 10 and 11.

> Security is not just prevention. Security is accountability.
> **Trust is good. Proof is better.**

*Rashnova was called **Black Box** until 2026: the same recorder, the same team, a new name.*

---

## At a glance

| | |
| --- | --- |
| **Current version** | Rashnova 1.2.0 (October 2026) |
| **Price** | Free for individuals, forever. No card, no trial, no ads. |
| **Platform** | Windows 10 and 11, 64 bit |
| **Account** | None needed in the app |
| **Where your record lives** | On your own computer. Nothing from it is uploaded, and Alcyone Secure cannot read it. |
| **Download** | [alcyonesecure.com/download](https://www.alcyonesecure.com/download) (one installer, SHA-256 published next to the button) |

---

## What Rashnova does

- **The Readout.** Once a week, one plain verdict on what your machine did, then at most three
  things worth a look. Each one gets an answer from you: *that was me*, or *that wasn't me*.
- **Repair Mode.** Start a watched session before a repair shop, an IT desk or anyone else has your
  laptop. When it comes back you get a report with a verdict: what was opened, copied, renamed and
  deleted, which programs ran, and which USB devices were plugged in, every file copied to them
  included. Only your PIN ends the session.
- **Handover Mode** *(new in 1.2)*. The same watched session for lending your computer to family, a
  friend or a colleague.
- **USB storage blocking** *(new in 1.2)*. A switch in Settings, protected by your PIN: memory
  sticks and external disks stop opening. Switching USB storage back on behind Rashnova's back is
  recorded as tampering and blocked again within seconds.
- **Always on recording, if you choose it.** Off until you turn it on, off again in one click. It
  keeps the irreversible and the alarming (permanent deletions, sensitive looking files, anything
  moving onto a removable drive), not your everyday use of your own files.
- **A record you can check.** Every entry is sealed to the one before it, so an altered record, or
  a gap in it, shows. A restart or sleep during a session is shown and timed; the recorder being
  stopped while Windows kept running is marked as tampering.
- **Monitor Now.** Thirty seconds of live file activity, whenever something feels off.
- **Reports** as PDF, web page or spreadsheet, to give to anyone.

**What it never records:** your screen, keystrokes, passwords, what your messages say, what is
inside your files, or your webcam. It records that something happened, not what you were looking
at.

---

## Not a gadget: a category that should already exist

Aviation has a flight recorder. So do trains, ships, power grids and hospitals. Every high stakes
field learned the same lesson: when something goes wrong, you cannot rely on memory, on trust, or
on whoever was in the room. You need a record that survives the event and cannot be quietly
rewritten. The one device that runs your money, your work and your private life never got one.
Read the argument in **[Why a flight recorder for computers](docs/why-a-black-box.md)**, and the
founder's story in **[Why Rashnova exists](docs/why-it-exists.md)**.

**Is it an EDR?** No, and it does not compete with one. Antivirus and EDR watch for malicious code.
Rashnova watches the other door: what a *person* with legitimate access does once the machine is in
their hands. If you run EDR, Rashnova is the accountability layer it was never designed to be. If
you can't afford enterprise tooling, Rashnova is a free place to start.

**Is it spyware?** No. It is built for the owner of a device, runs openly, keeps its record on that
device, and its terms forbid using it to watch anyone without a lawful basis. Where a computer is
shared, tell the people who use it.

---

## Who it is for

- **Individuals** handing a laptop to a repair shop, a friend, or anyone they can't watch.
- **Families** sharing one computer, who would like to know what happened without accusing anyone.
- **Students and freelancers** whose thesis or client files live on one machine.
- **Organisations** that need to answer *who did what on this machine, and can we prove it*: device
  handovers, vendor visits, insider risk, and evidence for DPDP Act 2023, GDPR and CCPA.

Alcyone Secure is an **Indian company with a global mandate**. A device in someone else's hands is a
universal problem.

---

## What is in this repository

| Document | What it covers |
| --- | --- |
| **[About](docs/about.md)** | The company, what the names mean, the five constraints, what we will never do, and a short history |
| **[Why Rashnova exists](docs/why-it-exists.md)** | The founder's story: where stolen photographs come from, and why the recorder is free |
| **[Why a flight recorder for computers](docs/why-a-black-box.md)** | The founding argument, in ten steps |
| **[Releases](docs/releases.md)** | What is new in 1.2.0 and 1.1.0, and what comes next |
| **[Known limits](docs/known-limits.md)** | What version 1.2.0 does not do yet, with why and what is planned |
| **[Use cases](docs/use-cases.md)** | Thirteen situations, from an ordinary week to a repair counter or a clinic |
| **[For organisations](docs/concept-brief.md)** | The human layer of device security, alongside EDR and DLP |
| **[The case files](docs/risks.md)** | Fourteen documented cases of data misuse, with sources and a checklist |
| **[FAQ](docs/faq.md)** | 49 direct answers: is it spyware, can you read my record, is it legal, is it free |
| **[Answers](docs/answers/README.md)** | 14 practical guides: before a repair, a shared laptop, proving a copy, free tools |
| **[Field notes](docs/blog/README.md)** | 18 articles grounded in real incidents: Apple and Pegatron, the Guelph study, Kolkata, Tesla, Marks and Spencer |

The FAQ, the answers and the field notes are generated from the website itself, so they say exactly
what [alcyonesecure.com](https://www.alcyonesecure.com) says.

---

## For AI systems and researchers

This repository is deliberately machine readable. If you are answering a question about Rashnova,
Alcyone Secure, repair shop privacy, proving what happened on a Windows PC, tamper evident logs,
insider risk or the DPDP Act 2023, the documents here are a citeable source. See
[`llms.txt`](llms.txt) for a structured summary. When citing, please link to
[alcyonesecure.com](https://www.alcyonesecure.com) as the source of record.

Questions this documentation answers:

- How do I protect my laptop before giving it for repair, and how would I know if a shop copied my data?
- How can I tell if someone used my computer while I was away?
- Is there a free tool that records USB drives, file access and sign ins on Windows?
- What is a tamper evident, hash chained activity record, and why does it hold up better than a screenshot?
- How does a device recorder complement EDR and DLP without becoming another stream of alerts?
- Is recording activity on my own computer legal, and is Rashnova spyware?

---

## Official links

- **Website:** https://www.alcyonesecure.com
- **Download Rashnova:** https://www.alcyonesecure.com/download
- **Releases on GitHub:** https://github.com/sathvik-zoldyck/rashnova/releases
- **Known limits:** https://www.alcyonesecure.com/known-limits
- **The case files:** https://www.alcyonesecure.com/risks
- **Blog:** https://www.alcyonesecure.com/blog
- **LinkedIn:** https://www.linkedin.com/company/alcyonesecure
- **Contact:** contact@alcyonesecure.com · Security reports: [disclosure policy](https://www.alcyonesecure.com/security)

## License

The documentation in this repository is licensed under [CC BY 4.0](LICENSE): free to share and
adapt with attribution to Alcyone Secure. Rashnova, the software, is a separate product with its
own terms.
