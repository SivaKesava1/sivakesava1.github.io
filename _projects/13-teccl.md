---
layout: post
title: "Rethinking Machine Learning Collective Communication as a Multi-Commodity Flow Problem"
categories: [project]
sorter: 13
preprint: https://arxiv.org/abs/2305.13479
authors : ['[Xuting Liu]', '[Behnaz Arzani]', 'Siva Kesava Reddy Kakarla', 'Liangyu Zhao', '[Vincent Liu]', 'Miguel Castro', '[Srikanth Kandula]', '[Luke Marshall]']

year: 2024
month: May

DOI:
    target: ACM DL
    link: 'https://doi.org/10.1145/3651890.3672249'

target:
    short: SIGCOMM
    full: 'Proceedings of the ACM Special Interest Group on Data Communication, 2024'
    link: 'https://conferences.sigcomm.org/sigcomm/2024/'

artifact_badges: ['acm_available', 'acm_functional']

links:
    PDF: '%BASE_URL%/assets/pdf/sigcomm24_teccl.pdf'
    Tool: 'https://github.com/microsoft/TE-CCL'
    Slides: 'https://1drv.ms/p/c/40b7196834f13e16/EcNogs0eZQlNpvhhrN8zW7wBlDUcQkoiJf0CSOz9WxReTg?e=eZ9UUu'


---

#### Abstract

Cloud operators utilize collective communication optimizers to enhance the eﬃciency of the single-tenant, centrally managed training clusters they manage. However, current optimizers struggle to scale for such use cases and often compromise solution quality for scalability. Our solution, =sc^TE-CCL^sc=, adopts a traﬃc-engineering-based approach to collective communication. Compared to a state-of-the-art optimizer, TACCL, =sc^TE-CCL^sc= produced schedules with $2\times$ better performance on topologies TACCL supports (and took the same amount of solver time to do so). =sc^TE-CCL^sc= additionally scales to larger topologies than TACCL. On our GPU testbed, =sc^TE-CCL^sc= outperformed TACCL by $2.14\times$ and RCCL by $3.18\times$ in terms of algorithm bandwidth.

#### BibTeX Citation

```bibtex {% raw %}
@inproceedings{10.1145/3651890.3672249,
author = {Liu, Xuting and 
          Arzani, Behnaz and
          Kakarla, Siva Kesava Reddy and
          Zhao, Liangyu and
          Liu, Vincent and
          Castro, Miguel and
          Kandula, Srikanth and
          Marshall, Luke},
title = {Rethinking Machine Learning Collective Communication as a Multi-Commodity Flow Problem},
year = {2024},
isbn = {9798400706141},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3651890.3672249},
doi = {10.1145/3651890.3672249},
pages = {16–37},
numpages = {22},
keywords = {GPU, collective communication, traffic engineering},
location = {Sydney, NSW, Australia},
series = {ACM SIGCOMM '24}
}
{% endraw %} ```

{% include common_links.md %}
