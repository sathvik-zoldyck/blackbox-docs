# How do I check where a photo came from, or whether it was edited?

*EVIDENCE · updated 2026-10-15*

> **Short answer.** Look at what the file itself says, then at where else it appears. A photo may carry facts written by the camera (the date, the device, sometimes the place), but these are easy to edit and are stripped by most messaging apps. Newer cameras and editing apps can add Content Credentials (the C2PA standard), a signed record of where the picture came from and what was changed; when they are present and intact, they are the strongest sign you will get. A time stamp or a proof shows the file existed by a certain time. A reverse image search shows where the picture appeared before. None of these proves a picture shows the truth, and no detector can promise that either: read what the evidence says, and notice what is missing.

## What a photo can tell you about itself

Photo facts, often called EXIF, are written by the camera: when, on what device, and sometimes where. They are useful when they are there and easy to fake or remove, and WhatsApp, Instagram and most social apps remove them when a picture is shared.

Content Credentials are different: a signed record, added by a camera or an app that supports the C2PA standard, saying where the picture came from and which edits were made. If the credentials are present and their signature checks, the file has not been changed since they were signed. If they are missing, that proves nothing either way; most pictures today have none.

## When it existed

A trusted time stamp or a Bitcoin time stamp over the file's fingerprint shows the file existed, exactly as it is, by that moment. That is often the question that matters in a dispute: was this picture taken before or after something happened?

## Why there is no simple real or fake button

Tools that promise to detect edited or generated pictures make mistakes in both directions, and a confident wrong answer is worse than none. The honest approach is to collect what the file and its proofs say, check each one, and be clear about what could not be checked.

## A careful check

1. **Get the original file.** Ask for the file itself, not a screenshot or a forwarded copy. Forwarding strips facts and recompresses the picture.
2. **Read its Content Credentials, if any.** Use an app or site that reads C2PA. A valid signature means the file is unchanged since it was signed.
3. **Read its photo facts, with suspicion.** Dates and devices can be edited. Treat them as a claim, not a proof.
4. **Look for a time stamp or a proof.** If the person who took it made a proof, check it: it shows the file existed by a certain time.
5. **Search for earlier copies.** A reverse image search can show the same picture appearing earlier, somewhere else.

## Where Rashnova fits

Rashnova's Origin does the file side of this on Windows, for free: drop a file in and it says where it came from, whether it changed, and when it existed, from what the file and its proofs say: Content Credentials (C2PA), photo facts, time stamps (RFC 3161), Bitcoin (OpenTimestamps) and Rashnova proofs. It reads the file on your computer and uploads nothing. It reports what the evidence says, and says plainly when something cannot be relied on; it does not decide whether a picture is real.

**Related:** [How can I prove a file existed on a certain date, without paying?](./prove-a-file-existed-on-a-date.md) · [How do I prove someone copied files from my laptop?](./prove-someone-copied-files.md) · [What free tools show what happened on my Windows PC?](./free-tools-see-what-happened-on-windows-pc.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/check-where-a-photo-came-from](https://www.alcyonesecure.com/answers/check-where-a-photo-came-from). This copy is generated from the website; edit the website, not this file.*

