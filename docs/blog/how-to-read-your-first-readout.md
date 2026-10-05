# How to read your first Readout

*Guide · Aug 2026 · 6 min read*

> **In short:** The Readout opens with a verdict, not a table. Most weeks it says nothing unusual happened, and that is the normal result. Three things are worth understanding: what the notable items mean, why marking them as yours makes future Readouts quieter, and why a missing day is shown as missing rather than as zero.

In aviation, when investigators recover a flight recorder, the process of extracting and interpreting what is on it is called the readout. Rashnova borrows the term because this is the part where you open the record and find out what it says.

It arrives once a week, on a day you choose. It is designed to take about twenty seconds.

## 1. The verdict

The first line is a plain statement, and most weeks it reads something like *nothing unusual this week*. That is not a failure of the product: it is the expected result, and it is worth more than it looks. An assurance you can check is a different thing from an assurance you are given.

When something is worth your attention, the verdict says so instead, and names how many things.

## 2. The continuity line

Underneath: how long recording has run without interruption. *Recording uninterrupted since 2 February, 43 days.* If capture was interrupted, it says that plainly instead. A record with a gap in it is a different thing from a record without one, and you should not have to go looking to find out which you have.

## 3. At most three things worth a look

Never more than three. This is deliberate: research on digest products consistently finds that the most common complaint is having to dig through clutter, and that showing more does not produce more value. The curation is the feature.

What qualifies is narrow, and each one is provable from the log rather than inferred:

- A USB device connected for the first time ever.
- An application reading a sensitive folder for the first time.
- A boot with no sign in afterwards, the machine started, nobody logged in.
- A burst of file access far above normal in a short window.
- An interruption in capture.

> **Note the wording** The Readout says "34 file reads by Chrome under Documents", never "you opened 34 files". Background processes read files too. The distinction sounds pedantic until it matters, which is exactly when you would want it to have been accurate.

## 4. Was this you?

Every item carries two buttons: **That was me** and **That wasn't me**. This is the part most people skip on the first Readout and use every week after.

Marking something as yours stops it being raised again. Over a few weeks this matters enormously: the Readout learns what normal looks like *for you* and gets quieter, which is the opposite of what alerting tools usually do. Marking something as not yours takes you to the sealed evidence for that moment, which you can export.

Those labels never leave your machine. They are not uploaded, and they are not used to build a profile of you. They tune your Readout, on your computer.

## 5. The sealed line

At the bottom: how many log entries the Readout covers, and whether that range verified intact. Every entry in a Rashnova log is sealed to the entry before it, so altering one breaks every seal after it. The Readout checks that chain across the week it summarises and reports the result.

If the chain is broken anywhere in the window, the Readout marks itself unverified rather than presenting its counts as fact. That is unusual, and it is the point: a summary that would report the same numbers whether or not the underlying record had been tampered with is not evidence of anything.

## 6. What it cannot see

A permanent line at the foot states what the Readout covers: file reads, USB devices, processes, boots: and what it does not: screen content, keystrokes, network payloads, sleep and wake.

This is a feature rather than a disclaimer. Every product in this space implies it sees everything. Stating the boundary is what makes everything above the line believable, and it is the same principle the product is built on: trust is good, proof is better, and proof has edges.

## 7. Coverage

If part of the week is missing: logs rotated out, capture stopped, the Readout says so: *this Readout covers 4 of 7 days*. A day with no data is shown as no data, never as a zero. A quiet day and an unrecorded day look identical on a chart and mean completely different things, and conflating them would be the easiest lie in the product to tell.

## Questions

**How often does the Readout arrive?**

Once a week, on a day you choose. The default is Sunday. A local notification tells you it is ready; the Readout itself lives in the app.

**Is the Readout emailed to me?**

No. Emailing the substance of your week would contradict the local first design: it would put a readable summary of your activity on a mail server. If email notification is ever added it will say only that a Readout is ready, with no content, and it will be opt in.

**Can I turn the Readout off?**

Yes. It is on by default because most people want it, but it is a switch like everything else, and turning it off does not affect recording, your hash chain, or your reports.

**Why does it only show three items?**

Because a list of thirty is a list nobody reads. The value is in the selection, not the volume, and the full log is always available in the app for anyone who wants to go through it directly.

**Does the Readout tell me if I have been hacked?**

No, and it will not pretend to. It reports what the log shows: which programs read which folders, which devices connected, when the machine started. It does not classify anything as an attack, because it cannot do that honestly. It shows you what happened and leaves the judgement to you.

**Related**

- [How to see which apps are accessing your files on Windows](../answers/see-what-apps-access-my-files-windows.md)
- [Hash chains, explained for non cryptographers](./hash-chains-explained-non-cryptographer.md)
- [What was my computer doing while I was asleep?](../answers/what-was-my-computer-doing-overnight.md)

---

*Source of record: [https://www.alcyonesecure.com/blog/how-to-read-your-first-readout](https://www.alcyonesecure.com/blog/how-to-read-your-first-readout). This copy is generated from the website; edit the website, not this file.*

