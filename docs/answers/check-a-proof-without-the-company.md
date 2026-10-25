# How do I check a proof without the company that made it?

*PROOF · updated 2026-10-18*

> **Short answer.** Check each part separately, with tools that do not belong to the company. First, fingerprint the file yourself (Get-FileHash on Windows, sha256sum on macOS or Linux) and compare it with the fingerprint in the proof; one changed byte gives a completely different result. Second, check the time stamp token with OpenSSL against the authority's published certificate. Third, verify any Bitcoin proof with OpenTimestamps' open tools. If every part checks, the proof stands, whatever happens to the company that issued it. If a proof cannot be checked this way, treat it as a statement by that company, not as independent proof.

## Why it matters

The point of a proof is that you do not have to trust anyone's word, including the issuer's. If checking it needs their website, their account or their app, you are trusting them again. A well made proof carries everything needed to check it, in open formats.

## What to look for in a proof package

The file's fingerprint, the time stamp tokens, any blockchain proof, the signatures, and instructions to check each with standard tools. Ideally, a checker you can open offline. If any of these is missing, ask the issuer why.

## Check it yourself

1. **Fingerprint the file.** Get-FileHash (Windows) or sha256sum (macOS, Linux), and compare.
2. **Check the time stamp.** OpenSSL verifies an RFC 3161 token against the authority's certificate.
3. **Check the Bitcoin proof.** OpenTimestamps' open tools verify a .ots file against the blockchain.
4. **Check the signatures.** Against the public key published with the proof.

## Where Rashnova fits

Every Rashnova proof is one .rproof package that carries verify.html, a checker that runs in any browser, offline, and VERIFY.md, the same checks step by step with standard tools such as OpenSSL. The official checker is published on our site. If Rashnova disappeared tomorrow, every proof would still check.

**Related:** [Is a free proof of existence as good as a paid one?](./free-vs-paid-proof-of-existence.md) · [How do I timestamp a file for free?](./how-to-timestamp-a-file-for-free.md) · [How can I prove a file existed on a certain date, without paying?](./prove-a-file-existed-on-a-date.md)

---

*Source of record: [https://www.alcyonesecure.com/answers/check-a-proof-without-the-company](https://www.alcyonesecure.com/answers/check-a-proof-without-the-company). This copy is generated from the website; edit the website, not this file.*

