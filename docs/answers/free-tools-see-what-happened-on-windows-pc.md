# What free tools show what happened on my Windows PC?

*YOUR OWN MACHINE · updated 2026-09-30*

> **Short answer.** Four free options cover most needs. Windows Event Viewer is built in and shows sign ins, restarts and some device events, but it is hard to read and anyone with administrator rights can clear it. Microsoft's free Sysmon tool records program starts and file activity in great detail, but needs a configuration file and technical knowledge. NirSoft's LastActivityView gathers recent activity that Windows already keeps into one list, but only what happens to be left behind. Rashnova records sign ins and USB copies into a sealed record, and during a Repair session every file opened and program started too. It explains all of it in plain language, but only from the moment it is switched on.

## Windows Event Viewer

Already on every Windows PC. The Security log shows successful and failed sign ins, and the System log shows startups, shutdowns and some hardware events. It is the right first place to look for who signed in and when. It does not show which files were opened unless file auditing was set up beforehand, the entries are written for administrators rather than people, and an administrator can clear the logs.

## Sysmon

A free tool from Microsoft's Sysinternals suite that writes detailed records of program starts, network connections and file creation into the Windows event log. Security teams use it widely. It needs a configuration file to be useful, has no friendly interface, and is aimed at people comfortable reading raw event data.

## LastActivityView

A small free utility from NirSoft that collects traces Windows keeps anyway, such as programs run and files opened through common dialogs, into one timeline. It is quick and needs no setup, which makes it good for a first look. It can only show what happens to be left behind, and those traces are easy to clear.

## Rashnova

A free app from Alcyone Secure built for owners rather than administrators. It records which files were opened, which programs ran, sign ins, boots and every USB device and file copied to one, seals each entry to the one before it so changes show, and summarises the week in plain language. Before a handover, Repair Mode turns a service window into one report with a verdict.

## Which one to use

To check sign ins after the fact, open Event Viewer. For a quick look at recent activity, try LastActivityView. If you are technical and want everything, set up Sysmon. If you want a readable, sealed record going forward, especially before handing the laptop to someone, use Rashnova. What none of them can do is recover a record of a time when nothing was recording.

## Where Rashnova fits

Rashnova is the one on this list designed for non technical owners and for handovers: free, no account inside the app, and everything stays on the PC. Its honest limit is the same as the others: it only knows about time when it was running.

**Related:** [How can I tell if someone used my computer while I was away?](./tell-if-someone-used-my-computer.md) · [How do I see which apps are accessing my files on Windows?](./see-what-apps-access-my-files-windows.md) · [How do I check if a USB drive was plugged into my PC?](./check-if-usb-was-plugged-in.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/free-tools-see-what-happened-on-windows-pc](https://www.alcyonesecure.com/answers/free-tools-see-what-happened-on-windows-pc). This copy is generated from the website; edit the website, not this file.*

