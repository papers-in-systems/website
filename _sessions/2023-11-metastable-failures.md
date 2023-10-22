---
layout: session
title: Metastable Failures in the Wild
paper_title: Metastable Failures in the Wild
paper_author: Huang, et al.
paper_year: 2022
paper_link: https://www.usenix.org/conference/osdi22/presentation/huang-lexiang
presenter:
  - name: Juno Suárez
    link: https://hachyderm.io/@juno
registration: https://ti.to/bredemeyer/metastablefailures/
date: 2023-11-13
---

> Metastable failures are a class of system failures characterized by sustaining effects that keep systems in a degraded state and resist recovery.

> A key property of metastable failures is that their root cause is not a specific hardware failure or a software bug. It is an emergent behavior of a system, and it naturally arises from the optimizations for the common case that lead to sustained work amplification. As such, metastable failures are hard to predict, may potentially have catastrophic effects, and incur significant ongoing human engineering costs because automated recovery is difficult
