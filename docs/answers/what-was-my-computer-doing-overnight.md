# What was my computer doing while I was asleep?

*YOUR OWN MACHINE · updated 2026-08-20*

> **Short answer.** Some of it is visible. Event Viewer records the machine starting and stopping in the System log under event IDs 6005 and 6006, and Windows Update keeps its own installation history under Settings. What Windows does not give you is a readable account of which programs ran overnight and which files they touched: that data is either not retained or scattered across logs that are hard to read and easy to clear. Overnight activity is usually mundane: scheduled updates, search indexing, backup software, antivirus scans. Occasionally it is not. The dependable way to know either way is to record continuously and read a summary, rather than reconstructing the night from fragments.

## What you can reconstruct

Open Event Viewer and look at Windows Logs → System. Event ID 6005 marks the event log starting, which in practice means the machine booted; 6006 marks a clean shutdown. Filtering that log to the hours you were asleep gives you a rough shape of the night, whether the machine restarted, and when.

Settings → Windows Update → Update history shows what was installed and when, which explains a great many mysterious overnight restarts. Task Scheduler shows which scheduled tasks are configured to run and their last run time, which accounts for most remaining background activity: indexing, defragmentation, telemetry, backups.

## What you cannot

The gap is file activity. Windows does not, by default, keep a record of which programs read which files. That is not an oversight so much as a performance decision, the volume would be enormous, and the last access timestamp is disabled by default for the same reason.

So the specific question people usually mean, did anything read my documents while I was asleep, is not answerable from built in logs after the fact. You can see that a process ran. You generally cannot see what it touched.

## Before you worry

A machine that wakes at three in the morning, runs for six minutes and goes back to sleep is almost always doing maintenance. Windows schedules its automatic maintenance window overnight by design, and wake timers exist to allow it. Unexpected activity is worth understanding, but it is rarely sinister.

## Where Rashnova fits

Rashnova records continuously, including while you are asleep, so the question becomes answerable rather than speculative. Its weekly Readout reports which programs read which folders and how many times, which USB devices appeared, and how activity was distributed across each day of the week, with boot events shown alongside, so an overnight restart is visible in context. It reports what the log contains and nothing more: it will tell you that a program read a folder, not why. It is free, runs locally, and can be switched off if you would rather it did not run.

**Related:** [How do I see which apps are accessing my files on Windows?](./see-what-apps-access-my-files-windows.md) · [How can I tell if someone used my computer while I was away?](./tell-if-someone-used-my-computer.md) · [What free tools show what happened on my Windows PC?](./free-tools-see-what-happened-on-windows-pc.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/what-was-my-computer-doing-overnight](https://www.alcyonesecure.com/answers/what-was-my-computer-doing-overnight). This copy is generated from the website; edit the website, not this file.*

