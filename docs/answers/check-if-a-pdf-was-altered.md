# How can I check if a PDF has been altered?

*PROOF · updated 2026-10-22*

> **Short answer.** It depends on what you have to compare against. If the PDF is digitally signed, open it in a PDF reader and check the signature panel: it tells you whether the document changed after it was signed. If you have the original file, compare fingerprints: Get-FileHash in PowerShell gives the SHA-256, and one changed byte gives a completely different result. If the PDF was proved, check it against its proof. File properties such as the modified date and the producing app give hints but are easy to edit. Without a signature, an original or a proof, you usually cannot be certain, which is why it pays to prove important documents the day you receive or sign them.

## Strong checks

A valid digital signature covers the document at the moment of signing; readers flag any change made afterwards. A matching fingerprint against a trusted original means the files are identical. A matching proof means the file is exactly the one that existed at the proof's time.

## Weak hints

Document properties (created and modified dates, the app that made it), odd fonts, misaligned text or mismatched dates can suggest editing, but none is reliable on its own, and all can be faked.

## For the documents that matter

1. **Prove it when you get it.** A contract, an invoice, a letter: prove it the day it arrives or the day you sign.
2. **Keep the original.** A printed and rescanned copy, or one saved again, no longer matches.
3. **Check against the proof later.** Matches, or does not match: no guessing.

## Where Rashnova fits

Rashnova Proof makes that first step free and offline: drop in the PDF and get a proof witnessed by four independent services, without the file leaving your computer. Later, drop the PDF and its proof in again (or into the checker in any browser) and it says plainly: matches, or does not match.

**Related:** [How can I prove a file existed on a certain date, without paying?](./prove-a-file-existed-on-a-date.md) · [How do I check a proof without the company that made it?](./check-a-proof-without-the-company.md) · [How do I timestamp a file for free?](./how-to-timestamp-a-file-for-free.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/check-if-a-pdf-was-altered](https://www.alcyonesecure.com/answers/check-if-a-pdf-was-altered). This copy is generated from the website; edit the website, not this file.*

