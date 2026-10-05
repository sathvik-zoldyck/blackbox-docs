# How do I see which apps are accessing my files on Windows?

*YOUR OWN MACHINE · updated 2026-08-20*

> **Short answer.** Windows has no built in view for this. Resource Monitor shows live file activity under its Disk tab, but only for the current moment, with no history and no way to read it at volume. Sysinternals Process Monitor captures far more, but produces tens of thousands of events per minute and is built for engineers debugging software. Windows also supports file system auditing through Group Policy, which writes to the Event Log, but it is off by default, must be configured folder by folder, and produces output most people will never read. For an ongoing, readable answer you need something that records continuously and then summarises it.

## The three built in options, honestly compared

Resource Monitor (run resmon, then the Disk tab) is the quickest. It lists processes with current read and write activity and the files involved. It is genuinely useful for 'what is hammering my disk right now', and useless for anything historical, close the window and the information is gone.

Process Monitor from Microsoft's Sysinternals suite is the powerful option. It captures file, registry, network and process events in enormous detail. The difficulty is volume: a quiet minute on an idle machine can produce fifty thousand events. Without filters and some knowledge of what normal looks like, it tells you very little.

File system auditing through Group Policy or auditpol is the closest thing to a real audit trail. You enable object access auditing, then set a System Access Control List on each folder you care about. Events land in the Security log. It works, it is fiddly to configure, it is unavailable in some Windows editions, and the Event Log can be cleared by an administrator.

## Why this is harder than it should be

On a phone, this problem is considered solved. iOS has an App Privacy Report showing which apps accessed your photos, microphone and location over the past seven days, in plain language, on the device. Android has similar visibility.

Windows never got an equivalent. The data is there, the operating system's own Event Tracing infrastructure is what professional tools read, but nothing collects it into something an ordinary owner can read on a Sunday afternoon.

## Where Rashnova fits

Rashnova is our answer to that gap. It records the same kinds of activity the professional tools look at, continuously once you switch it on, into a tamper evident log on your machine, and produces a weekly summary called the Readout: which programs read which folders and how often, which USB devices were seen, how activity was spread across the days. There is also Monitor Now, a thirty second scan showing what is touching your files right now. Both are free, both run locally, and nothing is uploaded to produce them. The Readout reports what the log shows: it does not guess at why a program read a folder.

**Related:** [What was my computer doing while I was asleep?](./what-was-my-computer-doing-overnight.md) · [How can I tell if someone used my computer while I was away?](./tell-if-someone-used-my-computer.md) · [What free tools show what happened on my Windows PC?](./free-tools-see-what-happened-on-windows-pc.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/see-what-apps-access-my-files-windows](https://www.alcyonesecure.com/answers/see-what-apps-access-my-files-windows). This copy is generated from the website; edit the website, not this file.*

