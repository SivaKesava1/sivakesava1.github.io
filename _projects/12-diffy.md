---
layout: post
title: "=sc^Diffy^sc=: Data-driven Bug Finding for Configurations"
categories: [project]
sorter: 12
authors : ['Siva Kesava Reddy Kakarla', '[Francis Y. Yan]', '[Ryan Beckett]']

year: 2024

DOI:
    target: ACM DL
    link: 'https://dl.acm.org/doi/10.1145/3656385'

target:
    short: PLDI
    full: 'Proceedings of the ACM on Programming Languages, Volume 8,  Issue PLDI (Programming Language Design and Implementation), 2024'
    link: 'https://pldi24.sigplan.org/'

artifact_badges: ['acm_available']

links:
    PDF: '%BASE_URL%/assets/pdf/pldi24_diffy.pdf'
    Tool: 'https://github.com/microsoft/DiffyConfigAnalyzer'
    Talk: 'https://www.youtube.com/watch?v=Bwg3jM50K6A'
    Slides: 'https://1drv.ms/p/c/40b7196834f13e16/IQPgSm7YjAmZRo8A5iHxaNlFAQphx8C6tSevSBdgqu2fVC0'

---


#### Abstract

Configuration errors remain a major cause of system failures and service outages. One promising approach to identify configuration errors automatically is to learn common usage patterns (and anti-patterns) using data-driven methods. However, existing data-driven learning approaches analyze only simple configurations (_e.g._, those with no hierarchical structure), identify only simple types of issues (_e.g._, type errors), or require extensive domain-specific tuning. In this paper, we present =sc^Diffy^sc=, the first push-button configuration analyzer that detects likely bugs in structured configurations. From example configurations, =sc^Diffy^sc= learns a common template, with “holes” that capture their variation. It then applies unsupervised learning to identify anomalous template parameters as likely bugs. We evaluate =sc^Diffy^sc= on a large cloud provider’s wide-area network, an operational 5G network testbed, and MySQL configurations, demonstrating its versatility, performance, and accuracy. During =sc^Diffy^sc=’s development, it caught and prevented a bug in a configuration timer value that had previously caused an outage for the cloud provider.

{% include common_links.md %}


#### BibTeX Citation

```bibtex {% raw %}
@article{10.1145/3656385,
author = {Kakarla, Siva Kesava Reddy and
          Yan, Francis Y. and
          Beckett, Ryan},
title = {Diffy: Data-Driven Bug Finding for Configurations},
year = {2024},
issue_date = {June 2024},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
volume = {8},
number = {PLDI},
url = {https://doi.org/10.1145/3656385},
doi = {10.1145/3656385},
journal = {Proc. ACM Program. Lang.},
month = {jun},
articleno = {155},
numpages = {24},
keywords = {anomaly detection, configuration bug finding, template synthesis}
}
{% endraw %} ```