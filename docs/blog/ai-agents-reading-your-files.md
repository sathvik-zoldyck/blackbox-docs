# Your AI assistant just read your Documents folder. Would you know?

*Security · Aug 2026 · 8 min read*

> AI agents work by reading and writing files with your privileges. When one accesses a file it does not open it — it ingests it. Windows keeps no record of which one touched what.

An AI agent is a program you hand a goal to instead of an instruction. "Sort out these invoices." "Find the contract we signed in March." To do that, it reads and writes files on your machine, with your privileges, and — this is the part worth sitting with — **it decides which files to open.** You did not name them. It went looking.

That is not a criticism. It is how the tools work, and it is why they are useful. But it changes the question you should be able to answer about your own computer, and almost nobody can answer it yet.

## Reading is not what happens

One line from the current research on agent safety captures the difference better than anything we could write: when an AI agent accesses a file, it does not read it — **it ingests it.** It scans, parses, and in many configurations transmits the contents to an external model for processing.

A human opening the wrong document glances at it and closes it. An agent opening the wrong document may have already sent it somewhere. The failure modes are not comparable, and the speed means there is no moment at which you could intervene.

Researchers describing this new paradigm put the problem plainly in a 2026 paper titled *Don't Let AI Agents YOLO Your Files* — the concern being that the agent, not the user, is now the one choosing what gets touched.

## The people building these things are the most worried

In the 2025 Stack Overflow Developer Survey, **81% of developers said they were concerned about the privacy and security of data when using AI agents.** That is not a public anxious about something it does not understand; that is the people who write the software.

Enterprise security research from 2026 describes the same thing as a governance gap: most organisations can see what their AI agents are doing, but the majority cannot stop them when something goes wrong. If that is the state of play inside companies with security teams, consider the state of play on a personal laptop.

## Windows Recall is the same problem, shipped by the platform

Recall, the Copilot+ PC feature that takes periodic snapshots of your screen so you can search them later, is instructive — not because it is malicious, but because of how the debate went.

Independent security testing when it first appeared raised serious questions about how the snapshot database was stored and how reachable it would be to anyone with access to the machine. After public backlash, Microsoft made the feature **opt-in rather than on by default**. Researchers have also documented that it captured content users believed was ephemeral, including disappearing messages in Signal and WhatsApp.

The lesson is not that Recall is uniquely bad. It is that a feature which quietly indexed everything on screen shipped as a default, and the correction came from public pressure rather than from anyone noticing on their own machine. Nobody could see it happening, so nobody could object on the evidence.

## What you cannot currently check

Ask the practical question — *which folders did that agent open last Tuesday?* — and Windows has no answer for you. The last-accessed timestamp is disabled by default for performance. File-system auditing exists but is off, must be configured per folder, and writes to a log an administrator can clear. Resource Monitor shows you this instant and keeps no history.

So the accountability position for AI agents on Windows today is roughly: you granted access, the agent used it, and there is no durable record of what it touched.

## What would settle it

Not blocking agents. They are useful, and a tool that fought them would be fighting the wrong thing. What is missing is much simpler: **a record of which program read which folder, when, that the owner can read and nobody can quietly edit.**

With that record, the interesting question becomes answerable rather than theoretical. Did the agent stay inside the project folder you pointed it at, or did it wander into the one with your tax returns? Did it start touching a new directory the week after an update? You do not need a threat classifier to find that useful — you need a log.

[Black Box](https://www.alcyonesecure.com/products/blackbox) keeps that log. It records file access at the kernel level into a hash-chained record on your machine, so which programs read which folders is something you can review afterward rather than guess at. It does not judge the agent. It keeps a record of where it went.

## Frequently asked

**Can I see which files an AI agent accessed on Windows?** Not with built-in tools, after the fact. Resource Monitor shows live activity with no history, Process Monitor produces far more detail than is readable, and file-system auditing is off by default and must be configured per folder. Unless something was recording at the time, the question cannot be answered retrospectively.

**Should I stop using AI agents?** That is not our argument. Agents are genuinely useful and the file access is what makes them work. The gap is that access was granted without visibility being granted alongside it. Being able to review what an agent touched is compatible with using one.

**Does Black Box block AI agents from reading files?** No. It is a recorder, not a blocker or a scanner. It records which programs read which folders so you can see it and, if it matters, prove it.

---

*Sources: [Don't Let AI Agents YOLO Your Files (arXiv, 2026)](https://arxiv.org/abs/2604.13536) · [Testing the privacy implications of Recall — Kevin Beaumont](https://doublepulsar.com/microsoft-recall-on-copilot-pc-testing-the-security-and-privacy-implications-ddb296093b6c). Published on the [Alcyone Secure blog](https://www.alcyonesecure.com/blog/ai-agents-reading-your-files). This document mirrors public website content for open, offline, and machine reading.*
