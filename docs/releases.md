# Releases

Rashnova is downloaded from **[alcyonesecure.com/download](https://www.alcyonesecure.com/download)**,
where the installer's SHA-256 is published next to the button. The installers themselves are
published on [GitHub](https://github.com/sathvik-zoldyck/rashnova/releases). Updates are announced
inside the app: once a day it checks for a newer version and tells you; you install it yourself, and
your record, PIN and settings are kept.

---

## Rashnova 1.3.0 (25 October 2026)

*Rebuilt from the first screen. And two new ways to trust a file.*

The biggest update yet: a completely new design, Rashnova Proof and Origin, a Repair Mode that
records far more of every visit, and a Handover Mode that keeps who has your computer.

- **A whole new design.** Every screen, from the very first one. One calm dark look, the brand
  orange only where you act, and the Seal turning slowly while Rashnova records.
- **Rashnova Proof.** Prove any file existed, exactly as it is, by a certain time. Witnessed by four
  independent clocks (drand, DigiCert, Sectigo and Bitcoin through OpenTimestamps), never by us.
  Signed twice, one signature post quantum. Free and offline: your file never leaves your computer,
  and anyone can check a proof in any browser, even without Rashnova, with the official checker at
  [alcyonesecure.com/proof](https://www.alcyonesecure.com/proof).
- **Origin.** Drop in a file to see where it came from, whether it changed and when it existed. It
  reads what the file says about itself and says plainly what cannot be relied on. Nothing is
  uploaded.
- **Repair Mode records far more.** During a session: folders opened in File Explorer, Wi‑Fi joined
  and left by name, and the title of a browser tab (never the address or what is on the page).
  Screenshots are named as such.
- **If someone tries to cover their tracks,** that is recorded too: clearing the recent files list,
  emptying the Recycle Bin, opening the browser's clear browsing data page.
- **What Windows itself says.** If Microsoft Defender finds something, or someone turns protection
  off, it is in your record, exactly as Windows wrote it.
- **Four clear levels.** Every row says Recorded, Worth a look, High or Critical, so a USB stick never
  looks the same as a private browser window.
- **Handover Mode keeps a ticket.** Who has the computer and why, what they used, and only your PIN
  takes it back. Past handovers are listed.
- **Always On, or only when you ask.** At setup you choose: Always On, quietly in the background, or
  only during a Repair or Handover session. Change it in one click.
- **It speaks up only when it matters.** Windows notifications for a few things only: a USB drive
  during a session, the recorder not answering, Monitor Now finished, a proof's Bitcoin time
  confirmed.
- **Updates inside the app.** Rashnova checks once a day and shows the new version's fingerprint
  before you install it.

**Upgrading:** install 1.3.0 over any earlier Rashnova. Your record, PIN and settings are kept.
**Downloading** needs a free account on the website; the app itself works without signing in.

---

## Rashnova 1.2.0 (October 2026)

*Lending your laptop? Hand it over, watched.*

This update adds Handover Mode and USB storage blocking, and makes restarts during a session read as
what they are. It is still the free local recorder: everything is recorded and kept on your
computer, and no account is needed.

- **Handover Mode.** For the times someone else uses your computer for a while: family, a friend, a
  colleague. It records exactly what Repair Mode records, with the same sealed report, and only your
  PIN ends it. It has its own button on the dashboard, its own page and its own button in the quick
  panel, and past sessions say which mode each one was.
- **A restart is not tampering.** A restart, a shutdown, a power cut or sleep during a session is
  shown in the report with its length, and no longer marks the session Compromised. The recorder
  being stopped while Windows kept running is recorded as tampering, and the session reads
  Compromised.
- **USB storage blocking.** Switch it on in Settings with your PIN, and memory sticks and external
  disks no longer open, fast USB 3 drives included. If someone switches USB storage back on outside
  Rashnova, that is recorded as tampering and it is blocked again within seconds.
- **Start with Windows.** Choose always on recording and Rashnova opens in the tray when you sign
  in, with no window, so Repair Mode and Handover Mode are a click away. It is its own switch in
  Settings too, and Windows lists it in its Startup apps, where you can turn it off.
- **PowerShell script logging only during a session.** Rashnova turns on Windows' PowerShell script
  logging when a Repair or Handover session starts and puts it back as it was when the session
  ends. 1.1.0 left it on between sessions.
- **Clearer words.** Change PIN says which step you are on. The Readout's cards say plainly what
  happened, every card can be opened, and a day marked partial is explained.
- **One file that installs itself.** The download is now a single installer (an MSI) that brings
  everything Rashnova needs, including its own copy of .NET 10. Nothing else is downloaded during
  setup and nothing needs to be installed first.

**Upgrading from 1.1.0:** download and install 1.2.0 over it. Your record, PIN and settings are kept,
and Rashnova appears once in Windows' installed apps list.

---

## Rashnova 1.1.0 (October 2026)

*The free local recorder. Black Box is now Rashnova.*

- **Repair Mode.** Start a watched session before you hand the PC over. When you get it back, you
  get a summary and a report of what was opened, copied, renamed and deleted, which programs ran,
  and which USB devices were plugged in, every file copied to them included.
- **Always on recording, if you choose it.** Off until you turn it on. It keeps the irreversible and
  the alarming (permanent deletions, sensitive looking files, anything moving onto a removable
  drive), not your everyday use of your own files. Turning it off never needs your PIN.
- **A record you can check.** Every entry is sealed to the one before it, so you can tell if the
  record was altered or has gaps.
- **The Readout.** Your week, in one verdict.
- **Monitor Now.** Thirty seconds of live file activity, whenever you want a look.
- **Reports** as PDF, web page or spreadsheet. What you save is a copy; the original stays where
  Rashnova keeps it.
- **No account.** The app needs no sign in at any point.

---

## Coming next

**Personal**, an optional paid plan, is coming soon: an encrypted copy of your record off the
computer, copies of your proofs in the cloud and longer history. It cannot be bought yet, and
everything above stays free. Anything else is announced when it ships.

*Source of record: [alcyonesecure.com/download](https://www.alcyonesecure.com/download).*
