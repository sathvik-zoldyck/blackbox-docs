# How do I check if a USB drive was plugged into my PC?

*YOUR OWN MACHINE · updated 2026-08-20*

> **Short answer.** Windows keeps a partial record. The registry key SYSTEM\CurrentControlSet\Enum\USBSTOR lists storage devices that have been connected, usually including vendor ID, product ID and serial number, and C:\Windows\INF\setupapi.dev.log records first-time device installations with timestamps. Between them you can often identify a drive that was connected and roughly when. Three limits matter: the registry generally preserves first and last connection rather than every one, both locations can be edited or cleared by an administrator, and neither records what was copied to or from the device. Tools such as USBDeview read the same data more conveniently but inherit exactly the same gaps.

## Reading the built in record

Open Registry Editor and navigate to HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Enum\USBSTOR. Each subkey represents a device class, and beneath it you will find instance identifiers that usually contain the device serial number. Properties under each instance can include friendly names and connection timestamps, though the exact layout varies by Windows version.

Then open C:\Windows\INF\setupapi.dev.log in a text editor and search for the vendor or product identifier. This file logs driver installation, so it typically captures the first time a particular device was attached, with a timestamp. NirSoft's USBDeview presents the same information in a table if you would rather not read the registry directly.

## The three things it will not tell you

First, it will not tell you what was transferred. Device connection and file copying are recorded, where they are recorded at all, by entirely separate mechanisms. A drive appearing in USBSTOR proves attachment, nothing more.

Second, it will not give you a complete timeline. The registry is a device database, not an event log; it is generally overwritten with the most recent connection rather than appended to.

Third, it is not tamper evident. Anyone with administrator rights can delete these keys or edit the log file, and doing so leaves no independent trace. For casual curiosity that is fine. For a dispute it is not.

## Where Rashnova fits

Rashnova records USB arrivals and removals as discrete timestamped events, each with vendor ID, product ID and serial where the device reports one, sealed into the same hash chain as everything else, so an entry cannot be removed without producing a visible break. Because arrivals and removals are separate events, you get a window rather than a single data point: this device was attached between these two times, while these files were being read. Its weekly Readout also reports whether anything was copied to removable media during the week. It is free, and it only covers time when it was running.

**Related:** [How can I tell if someone used my computer while I was away?](./tell-if-someone-used-my-computer.md) · [How do I prove someone copied files from my laptop?](./prove-someone-copied-files.md) · [How do I know if a repair shop copied my data?](./how-to-know-if-repair-shop-copied-data.md) · [How do I keep my privacy on a shared or family laptop?](./protect-privacy-on-shared-laptop.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/check-if-usb-was-plugged-in](https://www.alcyonesecure.com/answers/check-if-usb-was-plugged-in). This copy is generated from the website; edit the website, not this file.*

