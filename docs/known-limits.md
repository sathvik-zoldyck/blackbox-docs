# Rashnova 1.2.0: known limits

*What it does not do. Yet.*

A record is only worth trusting if you know where it stops. These are the limits of Rashnova 1.2.0
worth knowing before you install, each with why and what is planned.

## Installing

### 1. The installer is not code signed yet.

Your browser may hold the download back with "isn't commonly downloaded" or "unconfirmed". In Edge,
open Downloads, choose the three dots next to the file, then **Keep** and **Show more**, then
**Keep anyway**. In Chrome, open Downloads and choose **Keep**. When you run it, Windows SmartScreen
may show "Windows protected your PC" and "Unknown publisher": choose **More info**, then **Run
anyway**. Before you do, you can check that the file is the one we published: its SHA-256 is listed
next to the download link on [the download page](https://www.alcyonesecure.com/download).

- **Why:** we do not have a code signing certificate yet. Browsers and Windows trust a file by its
  publisher's signature, or by how many people have already downloaded that exact file. Every new
  version is a new file, so it starts with no history.
- **Planned:** a signed installer. Until then we report each new version to Microsoft when we
  publish it, and the warnings fade as people download it.

### 2. Windows only, 64 bit.

Rashnova 1.2.0 is built for 64 bit Windows 10 and 11, and has been tested on Windows 10. It brings
its own copy of Microsoft's .NET 10, used only by Rashnova: nothing else is downloaded during setup,
and nothing else needs to be installed first.

- **Planned:** nothing announced for other systems in this version.

## Your PIN

### 3. A forgotten PIN cannot be recovered.

Not by us, and not by signing in. Starting or ending a Repair or Handover session, exporting a
report and deleting data need the PIN. Switching off always on recording never needs it, so a
forgotten PIN can never keep you recorded all the time.

- **Why:** a way to recover the PIN would be a way around it for anyone who has the computer.
- **Planned:** nothing; this is deliberate.

## Who can read the record

### 4. The record can be read by the account that set the PIN, and by administrators.

The record on this computer can be read by the Windows account that set the Rashnova PIN and by
every administrator account on this computer. Other accounts cannot read it, and restarting the
computer or signing in with another account does not change that. The second copy is encrypted, and
Rashnova opens it only after your PIN is checked. The computer's administrators can still read it.

- **Why:** an administrator can change any permission on Windows, so no program can keep its files
  from one.
- **Planned:** nothing; this is how Windows works.

## What is recorded

### 5. Nothing can be recorded while the computer is off, asleep or restarting.

A Repair session ends only when you end it with your PIN. If the computer restarts, is switched off
or goes to sleep, or Rashnova's recorder is stopped during a session, recording pauses and resumes
by itself as soon as the computer starts or wakes again, before anyone signs in. The session's
report shows each interruption and how long it lasted. Nothing done in that time can be recorded. A
restart, a shutdown, a power cut or sleep is ordinary and does not count against the session.
Rashnova's recorder being stopped while Windows kept running counts as tampering, and the session
reads Compromised. After such a restart, Rashnova's encrypted copy of the record stays paused until
you enter your PIN.

- **Why:** nothing runs while the computer is off, and Rashnova opens the encrypted copy only after
  your PIN is checked.
- **Planned:** nothing; this is a deliberate trade.

## Not in this version

### 6. Cloud backup, sign in, recovery from another device, location recording and the paid plan.

1.2.0 is the free local recorder: everything is recorded and kept on this computer, with no account.
These features appear in Settings as "Coming soon".

- **Planned:** a later version.

## Updates

### 7. Updates are not installed automatically.

Once a day the app checks alcyonesecure.com for a newer version and tells you when there is one; you
download and install it yourself. Your record, PIN and settings are kept across an update. Security
fixes to Rashnova's copy of .NET come with Rashnova updates, not through Windows Update.

- **Planned:** nothing at present.

---

Found something that belongs here and is missing? Tell us at contact@alcyonesecure.com. Security
issues go through [our disclosure policy](https://www.alcyonesecure.com/security).

*Source of record: [alcyonesecure.com/known-limits](https://www.alcyonesecure.com/known-limits).*
