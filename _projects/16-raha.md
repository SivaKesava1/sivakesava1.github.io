---
layout: post
title: "=sc^Raha^sc=: A General Tool to Analyze WAN Degradation"
categories: [project]
sorter: 16
authors : ['[Behnaz Arzani]', 'Sina Taheri','[Pooria Namyar]', '[Ryan Beckett]', 'Siva Kesava Reddy Kakarla', 'Elnaz Jallilipour']

year: 2025

DOI:
    target: ACM DL
    link: 'https://doi.org/10.1145/3718958.3754348'

target:
    short: SIGCOMM
    full: 'Proceedings of the ACM Special Interest Group on Data Communication, 2025'
    link: 'https://conferences.sigcomm.org/sigcomm/2025/'


links:
    PDF: '%BASE_URL%/assets/pdf/sigcomm25_raha.pdf'
    Tool: 'https://github.com/microsoft/MetaOpt?tab=readme-ov-file#raha-instructions'
    Slides: 'https://1drv.ms/p/c/40b7196834f13e16/EfV25qxtl_BKpDHnLjMXa3kBwTrteZFTfP37-O-w7jVDAQ?e=bkoqm0'

    
---

#### Abstract

=sc^Raha^sc=  is the first general tool that can analyze probable _degradation_ of traffic engineered networks under _arbitrary_ failures and traffic shifts to prevent outages. =sc^Raha^sc=  addresses a significant gap in prior work which consider only (1) $\le k$ failures; (2) specific traffic engineering schemes; and (3) the maximum impact of failures irrespective of the network design point.

Our insight is to formulate the problem in terms of heuristic analysis, where one seeks to maximize the performance _gap_ between the network design point (_i.e.,_ the network with no failures) and the network under failures. We invent techniques that allow us to exploit the mechanisms within these tools to encode the problem into components which can handle them. We present extensive experiments on Microsoft's production network and those of Topology Zoo that demonstrate =sc^Raha^sc=  is scalable and can effectively solve the problem. We use =sc^Raha^sc=  to propose capacity augments that allow operators to mitigate potential problems and avoid future outages. Our results show =sc^Raha^sc=  can find $\ge 2\times$ higher degradations compared to those tools that only consider up to $2$ failures.

{% include common_links.md %}

#### BibTeX Citation

```bibtex {% raw %}
@inproceedings{10.1145/3718958.3754348,
    author = {Arzani, Behnaz and
              Taheri, Sina and
              Namyar, Pooria and
              Beckett, Ryan and
              Kakarla, Siva Kesava Reddy and
              Jalilipour, Elnaz},
    title = {Raha: A General Tool to Analyze WAN Degradation},
    year = {2025},
    isbn = {9798400715242},
    publisher = {Association for Computing Machinery},
    address = {New York, NY, USA},
    url = {https://doi.org/10.1145/3718958.3754348},
    doi = {10.1145/3718958.3754348},
    booktitle = {Proceedings of the ACM SIGCOMM 2025 Conference},
    pages = {184–202},
    numpages = {19},
    keywords = {traffic engineering, network performance analysis, network reliability},
    location = {S\~{a}o Francisco Convent, Coimbra, Portugal},
    series = {SIGCOMM '25}
}
{% endraw %} ```

