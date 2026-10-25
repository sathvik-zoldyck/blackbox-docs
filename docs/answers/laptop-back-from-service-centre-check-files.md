# My laptop came back from the service centre. How do I check if someone opened my files?

*AFTER THE FACT · updated 2026-10-25*

> **Short answer.** Look in seven places, in this order: the recent files list (press Windows + R and type recent), each browser's history, the Security log in Event Viewer for sign ins while it was away, the list of installed apps sorted by date, USB history, Windows Security's protection history, and the dates on your Photos and Documents folders. Together they can show that someone signed in, plugged in a drive or opened recent files. They cannot reliably show what was copied, and anyone with administrator rights can clear them, which technicians who snoop often do. If you find something, write it down with times and take photos of the screen before you use the laptop further. Next time, start a record before it goes.

## Why it is hard to be sure

Windows is not built to answer this question. It does not record which files were opened by default, and opening a photo leaves no lasting mark an ordinary user can find. In the University of Guelph's repair study, three of the six technicians who looked through customers' files then cleared Windows' recent files list, the first place most people check.

So treat everything below as clues. One clue means little. Several that point to the same time, a sign in at 11:40 at night, a USB drive at 11:42, recent files from your Pictures folder, tell a clearer story.

## If you find something, in India

Write down what you found, with dates and times, and photograph the screens. Then contact the service centre in writing, so there is a record of your complaint and their answer. If personal photos or data were taken or shared, you can report it at cybercrime.gov.in or on the 1930 helpline, and a dispute about the service itself can go to the consumer commission through e-Daakhil.

## Seven places to look

1. **Recent files.** Press Windows + R, type recent, press Enter. Sort by date modified and look at the days it was away. Also check Quick Access in File Explorer.
2. **Browser history.** Press Ctrl + H in each browser. Look for sites you did not visit while the laptop was away.
3. **Sign ins.** Event Viewer, Windows Logs, Security. Event 4624 is a sign in and 4625 a failed one. Look at the times the laptop was at the shop.
4. **Apps installed while it was away.** Settings, Apps, Installed apps, sort by date installed. Remote access or file recovery tools you did not install are worth asking about.
5. **USB drives.** On recent Windows versions, Event Viewer, Applications and Services Logs, Microsoft, Windows, Partition, Diagnostic lists drives that were connected. The registry key USBSTOR keeps a list too.
6. **Windows Security.** Virus and threat protection, Protection history: whether protection was turned off or anything was found while it was away.
7. **Your folders' dates.** In Photos, Documents and Desktop, sort by date accessed or modified and look for activity on the repair days.

## Where Rashnova fits

These checks only find what Windows happened to keep. Rashnova keeps the record on purpose: start Repair Mode before the next repair and every file and folder opened, every USB drive with each file copied to it, every program started, and any attempt to clear the recent files list is recorded and sealed, so the report you read afterwards cannot have been quietly edited. It cannot look back at a repair that already happened.

**Related:** [How do I know if a repair shop copied my data?](./how-to-know-if-repair-shop-copied-data.md) · [How do I check if a USB drive was plugged into my PC?](./check-if-usb-was-plugged-in.md) · [My data was leaked after a laptop or phone repair in India. What should I do?](./data-leaked-after-repair-india.md) · [How can I tell if someone used my computer while I was away?](./tell-if-someone-used-my-computer.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/laptop-back-from-service-centre-check-files](https://www.alcyonesecure.com/answers/laptop-back-from-service-centre-check-files). This copy is generated from the website; edit the website, not this file.*

