# Four witnesses, never us: how a Rashnova proof is witnessed, without the jargon

*Engineering · Oct 2026 · 8 min read*

> **In short:** A proof of time needs two edges: a moment the file cannot be older than, and a moment it must have existed by. Rashnova Proof gets the first from drand's public random values, and the second from two independent time stamp authorities and Bitcoin. Each witness sees only a salted fingerprint, none of them is us, and the proof checks itself offline.

Every proof of time has the same problem at its heart. You want to show when something existed, and the one clock you control, your own computer's, is the one clock nobody else has to believe. So a proof needs witnesses: clocks kept by others, who cannot be persuaded to say a different time, and who do not need to see your file.

Rashnova Proof uses four. This is what each one does, in plain words.

## First, what the witnesses actually see

None of them sees your file. Rashnova makes a fingerprint of the file on your computer (two, in fact: SHA-256 and SHA3-256), mixes in a random salt, and sends only that. A fingerprint cannot be turned back into the file, and the salt means nobody can even guess a well known file from its fingerprint. The witnesses learn that *something* was proved at a time, and nothing more.

## Witness one: drand, the edge called not before

drand is a public randomness beacon run by the League of Entropy, a group of independent organisations around the world. At a fixed rhythm it publishes a new random value, made jointly so that no single member can predict or choose it.

Rashnova puts the latest of those values into your proof. Because the value did not exist until a known moment, and nobody could have guessed it, the proof cannot have been made before that moment. This is the **not before** edge, and it closes a trick that time stamps alone leave open: making a proof today and claiming it is from long ago.

## Witnesses two and three: DigiCert and Sectigo, the edge called not after

A time stamp authority is a service whose job is to sign a statement: *this fingerprint existed at this time*. The format is a long standing internet standard, RFC 3161, readable by standard tools for decades to come.

Rashnova asks two separate authorities, DigiCert and Sectigo. Each signs your fingerprint with its own key and its own clock. This is the **not after** edge: the file existed, exactly as it is, by then. Two are asked so that the proof does not depend on any one company, or any one key, staying trustworthy forever.

## Witness four: Bitcoin, a ledger nobody can quietly rewrite

The fourth witness is the most public of all. Through OpenTimestamps, your fingerprint is folded into a Bitcoin transaction, and once that is in a block, changing it would mean rewriting the ledger that thousands of computers keep copies of.

It is slower: confirmation usually comes within a few hours, and the app tells you quietly when it has. Until then the proof says the Bitcoin time is on its way, and it is already complete with the other three.

> **Why four, and not one** Any single witness can disappear, change its rules or be doubted. Four independent ones, of three different kinds, mean a proof does not rest on anyone's continued good behaviour, including ours. That is the whole point of *never us*: Alcyone Secure is not one of the witnesses.

## Two signatures, one made for the future

The finished proof is signed on your computer twice: with ECDSA (P-256), the signature most of today's internet uses, and with ML-DSA-65, a post quantum signature standardised by NIST in FIPS 204. If computers powerful enough to break today's signatures ever arrive, the second one still holds.

## Checking it, years from now, without us

Every proof carries its own checker, a single page that runs in any web browser offline, and a plain text guide that repeats each check with standard tools. Drop in the file and the proof, and every character of both fingerprints is compared, every signature verified, every witness's statement checked. The result is *Matches* or *Does not match*, with nothing to sign in to and nothing sent anywhere.

If Rashnova disappeared tomorrow, your proofs would still check. A proof that needs its maker to survive is not much of a proof.

## What the four witnesses do not do

They witness a fingerprint and a time. They do not know or vouch for who you are, who made the file, or whether its contents are true, and Rashnova never says otherwise. A proof shows that this exact file existed, unchanged, by a certain time. That is a narrow claim, and it is one you can rely on.

## Questions

**What does not before and not after mean in a proof?**

Not before is the earliest the proof could have been made, set by a public random value nobody could know in advance (drand). Not after is the time by which the file must have existed, signed by time stamp authorities and Bitcoin.

**What is an RFC 3161 time stamp?**

A signed statement from a time stamp authority that a fingerprint existed at a certain time, in a long standing internet standard. Rashnova Proof gets two, from DigiCert and Sectigo.

**Why use Bitcoin for a time stamp?**

Once a fingerprint is in a Bitcoin block, changing it would mean rewriting a public ledger kept by thousands of computers. Through OpenTimestamps it adds a witness that no company controls. It usually confirms within a few hours.

**Does Alcyone Secure witness my proofs?**

No. The witnesses are drand, DigiCert, Sectigo and Bitcoin. We are deliberately not one of them, and checking a proof never needs us.

**What is a post quantum signature?**

A signature designed to stay secure even against future quantum computers. Each Rashnova proof is signed with ML-DSA-65 (NIST FIPS 204) as well as with ECDSA.

**Read next**

- [How to prove a file existed on a certain date](./how-to-prove-a-file-existed-on-a-date.md)
- [Hash chains, explained for non cryptographers](./hash-chains-explained-non-cryptographer.md)
- [Check a proof without the company](../answers/check-a-proof-without-the-company.md)
- [Rashnova Proof](https://www.alcyonesecure.com/proof)

---

*Source of record: [https://www.alcyonesecure.com/blog/four-witnesses-how-a-rashnova-proof-is-witnessed](https://www.alcyonesecure.com/blog/four-witnesses-how-a-rashnova-proof-is-witnessed). This copy is generated from the website; edit the website, not this file.*

