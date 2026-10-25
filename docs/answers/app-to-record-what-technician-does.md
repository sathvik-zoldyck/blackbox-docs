# Is there an app that records what a technician does on my laptop?

*BEFORE A HANDOVER · updated 2026-10-25*

> **Short answer.** Yes, but most tools built for this were made for something else. Screen recorders capture everything on screen, including your own private files, and stop the moment someone notices them. Windows' own file auditing can log access, but it has to be switched on folder by folder and the log can be cleared by any administrator. Free viewers such as NirSoft's LastActivityView only read traces Windows already keeps. Employee monitoring software records screens and keystrokes and is made for employers, not owners. What you want for a repair is narrower: a record of what was opened, copied, plugged in and run, that keeps going if someone tries to stop it, and that cannot be edited afterwards.

## What each kind of tool is good for

Screen recording shows everything, which is the problem: it records your own private photos as they are opened, it uses a lot of space over a day in a shop, and it is easy to notice and close. Windows' audit policy is powerful and free, but it needs setting up on each folder you care about, it is not available as a simple switch on Windows Home, and the Security log it writes to can be cleared.

Forensic viewers like LastActivityView are excellent for a quick look afterwards, but they read what Windows left behind, which a careful person can remove. Monitoring suites made for companies capture screens and keystrokes; that is more than you need and not what they were designed for.

## What to look for

For a repair, a good recorder notes activity, not content: which files and folders were opened, which USB drive was plugged in and what was copied to it, which programs ran. It keeps working if someone tries to stop it, shows the gap if they do, and seals the record so a change afterwards would show. And it asks for your PIN, not theirs, to end the session.

## Where Rashnova fits

Rashnova was built for exactly this, and it is free. Repair Mode records files and folders opened, programs started, USB drives with every file copied to them, Wi-Fi joined, screenshots taken, and attempts to cover tracks such as emptying the Recycle Bin or clearing the recent files list. It never records your screen, your keystrokes or what is inside your files. If the recorder is stopped, Windows starts it again within seconds and the report shows the gap. Only your PIN ends the session.

**Related:** [Is there a maintenance mode for Windows laptops, like Samsung's?](./windows-laptop-maintenance-mode.md) · [What free tools show what happened on my Windows PC?](./free-tools-see-what-happened-on-windows-pc.md) · [How do I protect my laptop before giving it for repair?](./protect-laptop-before-repair.md) · [Is Rashnova safe? Is it spyware?](./is-rashnova-safe.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/app-to-record-what-technician-does](https://www.alcyonesecure.com/answers/app-to-record-what-technician-does). This copy is generated from the website; edit the website, not this file.*

