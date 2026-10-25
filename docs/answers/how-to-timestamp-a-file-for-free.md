# How do I timestamp a file for free?

*PROOF · updated 2026-10-18*

> **Short answer.** Fingerprint the file on your own computer, then have that fingerprint witnessed by someone you do not control. The fingerprint (a SHA-256 hash) changes completely if one byte changes, so it pins down this exact version without the file ever leaving your machine. For the time, two free witnesses are trusted worldwide: a time stamp authority, which signs the fingerprint and the time under the internet standard RFC 3161, and OpenTimestamps, which writes it into a Bitcoin block within a few hours. Use both: two independent witnesses are far harder to argue with than one. Keep the original file and its time stamps together, and check them once straight away, while you can still fix anything.

## What a timestamp really proves

A trusted timestamp proves that this exact file existed no later than a certain moment. It does not prove when the file was created, who made it, or that what it says is true. That narrow promise is exactly why it holds up: it claims nothing it cannot show.

The file's date in Windows is not a timestamp in this sense. Anyone can change it in seconds, and it changes by itself when a file is copied.

## The free witnesses, and how they differ

Time stamp authorities are companies whose whole business is trusted time. Several run free public servers, used every day to time stamp signed software. The answer is a signed token that anyone can check with standard tools such as OpenSSL.

OpenTimestamps puts a fingerprint into the Bitcoin blockchain through free public servers. It depends on no single company, but it takes a few hours to confirm, and you keep a small proof file beside yours.

A public randomness beacon (drand, run by the League of Entropy) can show the other side: that a proof was not made before a certain time. Together, they give a window.

## Do it by hand, step by step

1. **Fingerprint the file.** In PowerShell, Get-FileHash gives the SHA-256. The file stays on your computer.
2. **Ask a time stamp authority.** Send only the fingerprint in an RFC 3161 request, and keep the signed reply.
3. **Add Bitcoin.** Stamp the same fingerprint with OpenTimestamps and keep the .ots file; upgrade it once the block confirms.
4. **Store everything together.** The file, the reply and the .ots file belong side by side, backed up together.
5. **Verify now.** Check both stamps today, so you know the proof works before you ever need it.

## Where Rashnova fits

Rashnova Proof does every step above in one drop, free, on Windows: two fingerprints (SHA-256 and SHA3-256), two independent time stamp authorities, Bitcoin through OpenTimestamps and drand, two signatures (one post quantum), and a certificate. The file never leaves your computer, and each proof carries its own checker that works in any browser, offline.

**Related:** [How can I prove a file existed on a certain date, without paying?](./prove-a-file-existed-on-a-date.md) · [Is a free proof of existence as good as a paid one?](./free-vs-paid-proof-of-existence.md) · [How do I check a proof without the company that made it?](./check-a-proof-without-the-company.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/how-to-timestamp-a-file-for-free](https://www.alcyonesecure.com/answers/how-to-timestamp-a-file-for-free). This copy is generated from the website; edit the website, not this file.*

