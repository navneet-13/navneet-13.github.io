---
layout: page
title: The Maya Cache — Secure Fully-Associative LLC
description: A storage-efficient, secure last-level cache that mitigates eviction-based side-channel attacks.
img:
importance: 4
category: research
related_publications: maya
---

**Advisor:** Prof. Biswabandan Panda, IIT Bombay &nbsp;·&nbsp; **Jan 2023 – Mar 2024**
&nbsp;·&nbsp; *Published at ISCA '24*

The Maya Cache is a secure, storage-efficient shared last-level cache (LLC) that mitigates
eviction-based side-channel attacks.

- Decoupled tag and data store with **pointer-based indirection** for **0% storage overhead**
  over the non-secure baseline LLC, with minimal performance impact.
- Motivated by the Reuse cache and Mirage cache, reducing data-store size by **50%** while
  keeping security comparable to Mirage without hurting performance.
