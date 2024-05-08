---
layout: post
title: "Rethinking Machine Learning Collective Communication as a Multi-Commodity Flow Problem"
categories: [project]
sorter: 13
preprint: https://arxiv.org/abs/2305.13479
authors : ['[Xuting Liu]', '[Behnaz Arzani]', 'Siva Kesava Reddy Kakarla', 'Liangyu Zhao', '[Vincent Liu]', 'Miguel Castro', '[Srikanth Kandula]', '[Luke Marshall]']

year: 2024
month: May


target:
    short: SIGCOMM
    full: 'Proceedings of the ACM Special Interest Group on Data Communication, 2024'
    link: 'https://conferences.sigcomm.org/sigcomm/2024/'


---

#### Abstract

Current optimizers for collective communication in distributed machine training fail to scale to the level needed by today's cloud operators and/or sacrifice solution quality significantly in pursuit of that scalability. Without such optimizers, GPU clusters spend significant time with idle GPUs and wasted resources.

=sc^TE-CCL^sc= takes a traffic engineering-based approach to collective communication. Compared to a state-of-the-art optimizer, TACCL, =sc^TE-CCL^sc= produced schedules with $2×$ better performance on topologies TACCL supports (and took the same amount of time to do so). =sc^TE-CCL^sc= also scales to larger topologies compared to TACCL. On our GPU testbed, =sc^TE-CCL^sc= outperformed TACCL by $2.14×$ and RCCL by $3.18×$.
    
{% include common_links.md %}
