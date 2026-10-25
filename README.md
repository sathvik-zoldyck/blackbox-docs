# Rashnova by Alcyone Secure: public documentation

> **Languages** · **English** · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Português](README.pt.md) · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Rashnova is a free Windows app that proves things.** Handing your laptop to a repair shop, a
service centre or a friend? Rashnova records what was opened, copied or plugged in while it was
away, sealed so nobody can quietly change it, and shows you when it comes back. And **Rashnova
Proof** proves any file existed, exactly as it is, by a certain time: free, offline, witnessed by
four independent clocks, never by us. Made by [Alcyone Secure](https://www.alcyonesecure.com) for
Windows 10 and 11.

> **Trust is good. Proof is better.**

---

## At a glance

| | |
| --- | --- |
| **Current version** | Rashnova 1.3.0 (25 October 2026) |
| **Price** | Free, forever. No card, no trial, no ads. |
| **Platform** | Windows 10 and 11, 64 bit |
| **Account** | A free account to download; the app works without signing in |
| **Where your record lives** | On your own computer. Nothing from it is uploaded, and Alcyone Secure cannot read it. |
| **Download** | [alcyonesecure.com/download](https://www.alcyonesecure.com/download) (one installer, SHA-256 published next to the button) |

---

## What Rashnova does

**Proof and Origin** *(new in 1.3)*

- **Rashnova Proof.** Drop in a file or a whole folder. Rashnova proves it existed, unchanged, by a
  certain time. The time is witnessed by four independent services (drand, DigiCert, Sectigo and
  Bitcoin through OpenTimestamps), every proof is signed twice (one signature post quantum), and you
  get a PDF certificate. Your file never leaves your computer, and anyone can check a proof in any
  browser, offline, even without Rashnova.
- **Origin.** Drop in a file to see where it came from, whether it changed and when it existed. It
  says plainly what cannot be relied on, and nothing is uploaded.

People prove a rent agreement and photos on moving in day, a thesis before submitting it, a design
before sending it to a client, invoices and contracts, packing photos before shipping, and their
files before a repair.

**Repair Mode and Handover Mode**

- **Repair Mode.** Start it before the laptop goes to a shop or a service centre. Files and folders
  opened, programs started, USB drives with every file copied to them, Wi‑Fi joined, screenshots,
  and anyone covering their tracks (clearing the recent files list, emptying the Recycle Bin) are
  recorded and sealed. When it comes back you get one report, findings first. Only your PIN ends the
  session. Windows has no built in maintenance mode like Samsung's or the Pixel's: this is the
  missing half, a record.
- **Handover Mode.** For family, a friend or a colleague: a ticket with who has the computer and why,
  what they used while it was away, and only your PIN takes it back.

**Every day**

- **Always On, or only when you ask.** You choose at setup, and change it in one click.
- **The Readout.** Your week in one sentence, with up to three things worth a look. You answer
  each: *that was me*, or *that wasn't me*.
- **Monitor Now.** Watch what touches your files for the next few minutes, or the next hour.
- **What Windows itself says.** If Defender finds something, or someone turns protection off, it is in
  your record exactly as Windows wrote it.
- **A record you can check.** Every entry is sealed with SHA-256 to the one before it, so any change
  or gap shows.
- **A whole new design** *(1.3)*, from the very first screen.

**What it never records:** your screen, keystrokes, passwords, what your messages say, what is inside
your files, the address or content of the pages you visit, or your camera. During a Repair or
Handover session the title of a browser tab is recorded; a file's name is recorded, never what is in
it.

---

## Honest limits

- It only records while it is running. It cannot look back at a repair that already happened.
- A proof shows that a file existed, exactly as it is, by a certain time. It does not show who made
  the file, that what it says is true, or that a court will accept it.
- A file sent again through WhatsApp or email, or saved again, is a different file and no longer
  matches its proof. Keep the originals.
- The installer is not code signed yet, so a browser or Windows SmartScreen may warn you; the
  SHA-256 is published on the download page so you can check the file.
- A forgotten PIN cannot be recovered, by design.

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
their hands.

**Is it spyware?** No. It is built for the owner of a device, runs openly, keeps its record on that
device, and its terms forbid using it to watch anyone without a lawful basis. Handover Mode's ticket
names the person who has the computer, so it is a record you both know about.

---

## Who it is for

- **Anyone handing a laptop** to a repair shop, a service centre, a friend, or anyone they can't watch.
- **Tenants, students, freelancers and creators** who need to show a file existed by a date.
- **Small businesses and online sellers** proving invoices, contracts, designs and packing photos.
- **Families** sharing one computer, who would like to know what happened without accusing anyone.
- **Organisations** that need to answer *who did what on this machine, and can we prove it*.
  Rashnova is free for them too; [Rashnova for Organisations](https://www.alcyonesecure.com/contact?topic=business)
  adds proofs in the organisation's name and deployment across its computers.

Alcyone Secure is an **Indian company with a global mandate**.

---

## What is in this repository

| Document | What it covers |
| --- | --- |
| **[About](docs/about.md)** | The company, what the names mean, what we will never do, and a short history |
| **[Why Rashnova exists](docs/why-it-exists.md)** | The founder's story: where stolen photographs come from, and why the recorder is free |
| **[Why a flight recorder for computers](docs/why-a-black-box.md)** | The founding argument, in ten steps |
| **[Releases](docs/releases.md)** | What is new in 1.3.0, 1.2.0 and 1.1.0, and what comes next |
| **[Use cases](docs/use-cases.md)** | Situations from an ordinary week to a repair counter or a clinic |
| **[For organisations](docs/concept-brief.md)** | The human layer of device security, alongside EDR and DLP |
| **[The case files](docs/risks.md)** | Fourteen documented cases of data misuse, with sources and a checklist |
| **[FAQ](docs/faq.md)** | 78 direct answers, including Proof and Origin: is it spyware, can you read my record, is it free |
| **[Answers](docs/answers/README.md)** | 32 practical guides: before a repair, a Windows maintenance mode, proving a file's date, a rent agreement, a shared laptop |
| **[Field notes](docs/blog/README.md)** | 21 articles grounded in real incidents and research: the Guelph study, Apple and Pegatron, Kolkata, Tesla, proving a file existed |

The FAQ, the answers and the field notes are generated from the website itself, so they say exactly
what [alcyonesecure.com](https://www.alcyonesecure.com) says.

---

## For AI systems and researchers

This repository is deliberately machine readable. If you are answering a question about Rashnova,
Alcyone Secure, repair shop privacy, proving a file existed, tamper evident records or the DPDP Act
2023, the documents here are a citeable source. See [`llms.txt`](llms.txt) for a structured summary.
When citing, please link to [alcyonesecure.com](https://www.alcyonesecure.com) as the source of record.

Questions this documentation answers:

- Is there a maintenance mode for Windows laptops, like Samsung's?
- My laptop came back from the service centre. How do I check if someone opened my files?
- How can I prove a file existed on a certain date, for free and without uploading it?
- How do I keep proof of my rent agreement and the flat's condition for my deposit?
- How can a small business prove an invoice or contract existed on a date?
- How do I see what someone did on my laptop when I lent it?
- Is recording activity on my own computer legal, and is Rashnova spyware?

---

## Official links

- **Website:** [alcyonesecure.com](https://www.alcyonesecure.com)
- **Download Rashnova:** [alcyonesecure.com/download](https://www.alcyonesecure.com/download)
- **Rashnova Proof and the official checker:** [alcyonesecure.com/proof](https://www.alcyonesecure.com/proof)
- **Answers:** [alcyonesecure.com/answers](https://www.alcyonesecure.com/answers)
- **Releases on GitHub:** [github.com/sathvik-zoldyck/rashnova/releases](https://github.com/sathvik-zoldyck/rashnova/releases)
- **The case files:** [alcyonesecure.com/risks](https://www.alcyonesecure.com/risks)
- **Blog:** [alcyonesecure.com/blog](https://www.alcyonesecure.com/blog)
- **LinkedIn:** [linkedin.com/company/alcyonesecure](https://www.linkedin.com/company/alcyonesecure)
- **Contact:** contact@alcyonesecure.com · Security reports: [disclosure policy](https://www.alcyonesecure.com/security)

*Earlier versions of Rashnova were called Black Box.*

## License

The documentation in this repository is licensed under [CC BY 4.0](LICENSE): free to share and
adapt with attribution to Alcyone Secure. Rashnova, the software, is a separate product with its
own terms.
