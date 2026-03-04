---
layout: post
title: "=sc^MetaEase^sc=: Heuristic Analysis from Source Code via Symbolic-Guided Optimization"
categories: [project]
sorter: 18
authors : ['[Pantea Karimi]', 'Siva Kesava Reddy Kakarla', '[Pooria Namyar]', '[Santiago Segarra]', '[Ryan Beckett]', '[Mohammad Alizadeh]', '[Behnaz Arzani]', ]

year: 2026

# DOI:
#     target: USENIX
#     link: 

target:
    short: NSDI
    full: 'Proceedings of the 23&hairsp;<sup>rd</sup> USENIX Symposium on Networked Systems Design and Implementation, 2026'
    link: 'https://www.usenix.org/conference/nsdi26'

artifact_badges: ['usenix_available', 'usenix_functional', 'usenix_reproduced']

links:
    PDF: '%BASE_URL%/assets/pdf/nsdi26_eywa.pdf'
    Tool: 'https://github.com/microsoft/MetaEase'
    # Slides: 
    # Talk:
---


#### Abstract

Large-scale systems rely on heuristics to tackle NP-hard problems such as traffic engineering, virtual machine placement, and packet scheduling. While these heuristics are efficient, they can exhibit severe performance gaps under certain workloads, leading to outages or costly over-provisioning. This risk has motivated tools that attempt to identify inputs causing worst-case underperformance. However, using these tools in practice often requires rewriting heuristics as formal mathematical models---a process that is time-consuming, error-prone, and excludes many real-world algorithms.

We introduce "=sc^MetaEase^sc=", a practical general-domain analyzer that works by directly analyzing a heuristic's source code, eliminating the need for formal modeling. =sc^MetaEase^sc= combines code-aware input generation with guided search to uncover worst-case scenarios efficiently, even for heuristics with randomness (_e.g.,_ various traffic engineering schemes) or non-convex behavior (_e.g.,_ bin packing for virtual machine placement).

Across five problem domains and eight heuristics, =sc^MetaEase^sc= matched or exceeded MetaOpt, a state-of-the-art optimization-based heuristic analyzer, in most cases; in the remainder, it achieved at least $85–98\%$ of its performance and often ran faster. Against black-box optimization baselines, it won in $88\%$ of settings and ranked in the top two otherwise. MetaEase analyzed Arrow, a widely studied networking heuristic, which cannot be analyzed by any of the state-of-the-art heuristic analyzers. We revealed previously unknown performance gaps in Arrow.

{% include common_links.md %}


#### BibTeX Citation

Coming soon!
