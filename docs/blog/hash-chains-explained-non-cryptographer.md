# Hash chains, explained for non-cryptographers

*Engineering · Apr 2026 · 6 min read*

> What a hash chain is, why it makes a log file tamper-evident, and what it does not do. A short, no-math explainer for product, security, and ops teams.

Hash chains are one of the most useful primitives in modern security, and one of the most under-explained. They sit underneath blockchains, audit logs, software supply-chain tooling, certificate transparency, and most forensic logging products. The concept itself is small.

## Start with the hash

A cryptographic hash function takes any blob of data and returns a fixed-length fingerprint. SHA-256 is the most common. Two useful properties: changing one byte of the input completely changes the output, and you cannot work backward from a fingerprint to a plausible input.

## Now chain them

A hash chain makes every entry depend on the entry before it. Each entry contains a header, a payload, and the hash of the previous entry. If an attacker edits entry 50, the hash of entry 50 changes, which breaks entry 51 prev-hash, which breaks 52, 53, and every entry after. The chain forces interference to be visible.

## Why this is forensic

Tamper-evident does not mean tamper-proof. The attacker can still delete the whole log. What they cannot do is edit one entry and leave the rest untouched. For a forensic recorder like [Black Box](https://www.alcyonesecure.com/products/blackbox), this is exactly the property you want.

## What hash chains are not

- They are not encryption. To keep payloads private, you encrypt them separately.
- They are not authentication. They prove that an entry has not been altered relative to its neighbours, not that the original writer was who they claimed to be.
- They are not blockchains. A blockchain is a distributed hash chain with a consensus mechanism on top.

## The two extra ingredients

- A shadow copy: an independent, encrypted second log written to a separate location.
- External anchors: periodic publication of the latest chain-tip hash to an outside system.

## When to use this

Use a hash chain whenever the integrity of an event log matters more than its secrecy. Audit logs in regulated environments, evidence chains in forensic recorders, change logs in supply-chain tooling. See how this fits into [forensic logging vs activity monitoring](./forensic-logging-vs-activity-monitoring.md).

**Q: Is a hash chain the same as a blockchain?**

No. A blockchain is a distributed hash chain with a consensus protocol. A local hash chain has no consensus; it relies on independent verifiers holding chain-tip values to detect deletion.

**Q: Can a hash chain be brute-forced?**

SHA-256 is not currently feasible to brute-force at any meaningful scale. The design assumes an adversary cannot find collisions.

---

*Published on the [Alcyone Secure blog](https://www.alcyonesecure.com/blog/hash-chains-explained-non-cryptographer). This document mirrors public website content for open, offline, and machine reading.*
