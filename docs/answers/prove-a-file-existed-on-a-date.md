# How can I prove a file existed on a certain date, without paying?

*EVIDENCE · updated 2026-10-15*

> **Short answer.** Fingerprint the file, then get that fingerprint witnessed by someone other than you. A fingerprint (a SHA-256 hash) changes completely if one byte of the file changes, so it pins down exactly this version. A witness pins down when. Free witnesses exist: public time stamp authorities sign a fingerprint with the time (the internet standard RFC 3161), and OpenTimestamps puts it into a Bitcoin block within a few hours. Emailing the file to yourself is better than nothing, but it rests on one provider's records. Whatever you use, keep the original file untouched: a copy resent through WhatsApp or email is recompressed and no longer matches. And remember what a proof cannot show: who made the file, or that what it says is true.

## What a proof of existence actually is

It is two facts tied together: this exact file, and a moment it already existed by. The file is reduced to a fingerprint, a short string that changes completely if anything in the file changes. The moment comes from a witness you do not control, so nobody has to take your word for the date.

That is also its limit. A proof of existence says nothing about who wrote the file, who owns it, or whether its content is true. Anyone selling more than that is selling more than the method can give.

## The common ways, honestly compared

Emailing the file to yourself gives you a date from your email provider. It is easy and free, but it rests on one company's records and on the account staying yours, and it is hard for anyone else to check independently.

A trusted time stamp (RFC 3161) is a signature from a time stamp authority over the file's fingerprint and the time. Several authorities offer this free for code signing, and the result can be checked with standard tools such as OpenSSL. It shows the file existed no later than that moment.

OpenTimestamps writes a fingerprint into a Bitcoin block. It is free and does not depend on any one company, but it takes a few hours to confirm and needs its small proof file kept beside yours.

Proof websites bundle these for you, usually for a fee per file or a subscription, and usually by uploading or hashing the file in their site. Ask two questions before paying: can the proof be checked without them, and does the file have to leave your computer?

## If you may need it as evidence

A proof shows when a file existed; whether a court accepts it is for the court. In India, an electronic record offered as evidence is usually accompanied by a certificate under Section 63 of the Bharatiya Sakshya Adhiniyam, 2023, which a lawyer or an expert prepares. Keep the original file, the proof, and a note of where the file came from. This is not legal advice.

## Do it properly

1. **Keep the original.** Prove the file as it came from the camera, the scanner or the signing, not a copy someone forwarded. Resending recompresses photos and breaks the match.
2. **Fingerprint it on your own computer.** On Windows, Get-FileHash in PowerShell gives the SHA-256. You do not need to upload the file anywhere to fingerprint it.
3. **Get the fingerprint witnessed by more than one party.** A time stamp authority and Bitcoin are independent of each other. Two witnesses are harder to argue with than one.
4. **Keep the proof with the file.** The proof is only useful next to the exact file it was made for. Back both up together.
5. **Check it once now.** Make sure the proof actually verifies today, while you still have everything needed to fix it.

## Where Rashnova fits

Rashnova Proof does all of this in one step, free, on Windows. Drop in a file or a whole folder; it fingerprints it on your computer (SHA-256 and SHA3-256), signs it twice, once with post quantum cryptography, and has the time witnessed by drand, two time stamp authorities (DigiCert and Sectigo) and Bitcoin, never by us. The file never leaves your computer, and every proof carries its own checker that works in any browser, offline, so anyone can check it without Rashnova. It does not prove who made the file or that a court will accept it.

**Related:** [How do I prove someone copied files from my laptop?](./prove-someone-copied-files.md) · [How do I check where a photo came from, or whether it was edited?](./check-where-a-photo-came-from.md) · [What is an evidence layer in cybersecurity?](./what-is-an-evidence-layer.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/prove-a-file-existed-on-a-date](https://www.alcyonesecure.com/answers/prove-a-file-existed-on-a-date). This copy is generated from the website; edit the website, not this file.*

