# Is there a maintenance mode for Windows laptops, like Samsung's?

*BEFORE A HANDOVER · updated 2026-10-25*

> **Short answer.** No. Windows has no built in equivalent of Samsung's Maintenance Mode or the Pixel's Repair mode, which hide your apps, photos and messages behind a temporary profile while the phone is being fixed. On a Windows laptop you can get part of the way yourself: give the technician a separate local account instead of your own, sign out of browsers and cloud drives, and back up first. That keeps routine work away from your files, but an administrator can still open any folder, and Windows keeps no readable record of what they did. The missing half is a record: something running during the repair that notes what was opened, copied or plugged in, sealed so it cannot be quietly edited.

## What phones do, and why laptops are different

Samsung added Maintenance Mode to Galaxy phones, and Google added Repair mode to Pixel phones with Android 14. Both work the same way: the phone restarts into a fresh, empty profile, the technician tests the repair there, and your data stays locked until you unlock it with your own PIN or fingerprint.

A laptop repair is often different. The technician may need to install drivers, run updates or test your own account, which needs administrator rights. Once someone has those, a separate profile does not stop them: an administrator can open any user's folders. So on Windows the realistic goal is two things together: keep routine work out of your account, and know afterwards what actually happened.

## What Windows can do today

A separate local account is the closest thing to Maintenance Mode. Create it in Settings, Accounts, Other users, give it a simple password for the technician, and keep your own account's password to yourself. BitLocker device encryption protects the drive if it is removed while the laptop is off, but not while it is running and unlocked, which is how a repair is tested.

None of this tells you what was done. Windows does not record which files were opened by default, and the few traces it does keep, like the recent files list, can be cleared in seconds.

## The closest thing to Maintenance Mode on Windows

1. **Back up, and check the backup opens.** Repairs sometimes reinstall Windows. Copy your files first and open a few from the copy.
2. **Make a separate account for the technician.** Settings, Accounts, Other users, Add account. Hand over that password, not yours.
3. **Sign out of what syncs.** Browsers, password managers, Google Drive, OneDrive, WhatsApp on the computer.
4. **Start a record before it leaves.** This is the part phones have and Windows lacks: a record of the visit you can read when it comes back.

## Where Rashnova fits

Rashnova adds the missing half for free. Start Repair Mode before the laptop leaves your hands: files and folders opened, programs started, USB drives and every file copied to them, Wi-Fi joined, and anyone clearing the recent files list are recorded and sealed, and only your PIN ends the session. When it comes back you get one report, findings first. It does not hide your files the way Samsung's mode does; it tells you what happened to them. Use it together with a separate account.

**Related:** [How do I protect my laptop before giving it for repair?](./protect-laptop-before-repair.md) · [Can repair shops see my photos?](./can-repair-shops-see-my-photos.md) · [My laptop came back from the service centre. How do I check if someone opened my files?](./laptop-back-from-service-centre-check-files.md) · [Is there an app that records what a technician does on my laptop?](./app-to-record-what-technician-does.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/windows-laptop-maintenance-mode](https://www.alcyonesecure.com/answers/windows-laptop-maintenance-mode). This copy is generated from the website; edit the website, not this file.*

