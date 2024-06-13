---
layout: post
title: "Rethinking Machine Learning Collective Communication as a Multi-Commodity Flow Problem"
categories: [project]
sorter: 13
preprint: https://arxiv.org/abs/2305.13479
authors : ['[Xuting Liu]', '[Behnaz Arzani]', 'Siva Kesava Reddy Kakarla', 'Liangyu Zhao', '[Vincent Liu]', 'Miguel Castro', '[Srikanth Kandula]', '[Luke Marshall]']

year: 2024
month: May

# DOI:
#     target: ACM DL
#     link: 'https://doi.org/10.1145/3651890.3672249'

target:
    short: SIGCOMM
    full: 'Proceedings of the ACM Special Interest Group on Data Communication, 2024'
    link: 'https://conferences.sigcomm.org/sigcomm/2024/'

links:
    PDF: '%BASE_URL%/assets/pdf/sigcomm24_teccl.pdf'

---

#### Abstract

Cloud operators utilize collective communication optimizers to enhance the eﬃciency of the single-tenant, centrally managed training clusters they manage. However, current optimizers struggle to scale for such use cases and often compromise solution quality for scalability. Our solution, =sc^TE-CCL^sc=, adopts a traﬃc-engineering-based approach to collective communication. Compared to a state-of-the-art optimizer, TACCL, =sc^TE-CCL^sc= produced schedules with $2\times$ better performance on topologies TACCL supports (and took the same amount of solver time to do so). =sc^TE-CCL^sc= additionally scales to larger topologies than TACCL. On our GPU testbed, =sc^TE-CCL^sc= outperformed TACCL by $2.14\times$ and RCCL by $3.18\times$ in terms of algorithm bandwidth.

#### BibTeX Citation

Soon!

{% include common_links.md %}
