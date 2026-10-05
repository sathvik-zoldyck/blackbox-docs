# Your AI assistant just read your Documents folder. Would you know?

*Security · Aug 2026 · 8 min read*

> **In short:** AI agents operate with your privileges and decide for themselves which files to open. Most people running one cannot say afterwards which folders it touched, because Windows does not keep that record. This is not an argument against agents: it is an argument for being able to see what they did.

An AI agent is a program you hand a goal to instead of an instruction. "Sort out these invoices." "Find the contract we signed in March." To do that, it reads and writes files on your machine, with your privileges, and: this is the part worth sitting with:**it decides which files to open.** You did not name them. It went looking.

That is not a criticism. It is how the tools work, and it is why they are useful. But it changes the question you should be able to answer about your own computer, and almost nobody can answer it yet.

## Reading is not what happens

One line from the current research on agent safety captures the difference better than anything we could write: when an AI agent accesses a file, it does not read it:**it ingests it.** It scans, parses, and in many configurations transmits the contents to an external model for processing.

A human opening the wrong document glances at it and closes it. An agent opening the wrong document may have already sent it somewhere. The failure modes are not comparable, and the speed means there is no moment at which you could intervene.

Researchers describing this new paradigm put the problem plainly in a 2026 paper titled *Don't Let AI Agents YOLO Your Files*, the concern being that the agent, not the user, is now the one choosing what gets touched.

## The people building these things are the most worried

In the 2025 Stack Overflow Developer Survey, **81% of developers said they were concerned about the privacy and security of data when using AI agents.** That is not a public anxious about something it does not understand; that is the people who write the software.

Enterprise security research from 2026 describes the same thing as a governance gap: most organisations can see what their AI agents are doing, but the majority cannot stop them when something goes wrong. If that is the state of play inside companies with security teams, consider the state of play on a personal laptop.

> **The gap, stated simply** Agents are being given file access faster than anyone is being given file visibility. The permission model advanced; the accountability model did not move at all.

## Windows Recall is the same problem, shipped by the platform

Recall, the Copilot+ PC feature that takes periodic snapshots of your screen so you can search them later, is instructive, not because it is malicious, but because of how the debate went.

Independent security testing when it first appeared raised serious questions about how the snapshot database was stored and how reachable it would be to anyone with access to the machine. After public backlash, Microsoft made the feature **opt in rather than on by default**. Researchers have also documented that it captured content users believed was ephemeral, including disappearing messages in Signal and WhatsApp.

The lesson is not that Recall is uniquely bad. It is that a feature which quietly indexed everything on screen shipped as a default, and the correction came from public pressure rather than from anyone noticing on their own machine. Nobody could see it happening, so nobody could object on the evidence.

## What you cannot currently check

Ask the practical question,*which folders did that agent open last Tuesday?*, and Windows has no answer for you. The last-accessed timestamp is disabled by default for performance. File-system auditing exists but is off, must be configured per folder, and writes to a log an administrator can clear. Resource Monitor shows you this instant and keeps no history.

So the accountability position for AI agents on Windows today is roughly: you granted access, the agent used it, and there is no durable record of what it touched. We have written up [the built in options and their limits](../answers/see-what-apps-access-my-files-windows.md) separately.

## What would settle it

Not blocking agents. They are useful, and a tool that fought them would be fighting the wrong thing. What is missing is much simpler: **a record of which program read which folder, when, that the owner can read and nobody can quietly edit.**

With that record, the interesting question becomes answerable rather than theoretical. Did the agent stay inside the project folder you pointed it at, or did it wander into the one with your tax returns? Did it start touching a new directory the week after an update? You do not need a threat classifier to find that useful: you need a log.

[Rashnova](https://www.alcyonesecure.com/products/rashnova) keeps that log. It records file access into a hash chained record on your machine, and the weekly [Readout](./how-to-read-your-first-readout.md) reports which programs read which folders, including the first time a program touches one, which is exactly the moment a new agent starts exploring. It does not judge the agent. It shows you where it went.

## Questions

**Can I see which files an AI agent accessed on Windows?**

Not with built in tools, after the fact. Resource Monitor shows live activity with no history, Process Monitor produces far more detail than is readable, and file system auditing is off by default and must be configured per folder. Unless something was recording at the time, the question cannot be answered retrospectively.

**Is Microsoft Recall a security risk?**

It became opt in rather than default on after public backlash, and independent testing raised questions about how its snapshot database was stored and reached. Researchers also documented it capturing content users expected to be ephemeral, including disappearing messages. Whether the current implementation is acceptable is a judgement call, the point worth taking is that nobody running it could see what it was doing on their own machine.

**Should I stop using AI agents?**

That is not our argument. Agents are genuinely useful and the file access is what makes them work. The gap is that access was granted without visibility being granted alongside it. Being able to review what an agent touched is compatible with using one.

**Does Rashnova block AI agents from reading files?**

No. It is a recorder, not a blocker or a scanner. It records which programs read which folders so you can see it and, if it matters, prove it. It makes no judgement about whether a given access was appropriate: that is yours to make.

**Sources and further reading**

- [Don't Let AI Agents YOLO Your Files (arXiv, 2026)](https://arxiv.org/abs/2604.13536)
- [Testing the security and privacy implications of Recall. Kevin Beaumont](https://doublepulsar.com/microsoft-recall-on-copilot-pc-testing-the-security-and-privacy-implications-ddb296093b6c)
- [Privacy and control over your Recall experience. Microsoft](https://support.microsoft.com/en-us/windows/privacy/privacy-and-control-over-your-recall-experience)
- [How to see which apps are accessing your files on Windows](../answers/see-what-apps-access-my-files-windows.md)

---

*Source of record: [https://www.alcyonesecure.com/blog/ai-agents-reading-your-files](https://www.alcyonesecure.com/blog/ai-agents-reading-your-files). This copy is generated from the website; edit the website, not this file.*

