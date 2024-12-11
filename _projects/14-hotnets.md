---
layout: post
title: "End-to-End Performance Analysis of Learning-enabled Systems"
categories: [project]
sorter: 14
authors : ['[Pooria Namyar]', '[Michael Schapira]', '[Ramesh Govindan]','[Santiago Segarra]', '[Ryan Beckett]', Siva Kesava Reddy Kakarla, '[Behnaz Arzani]']

year: 2024

DOI:
    target: ACM DL
    link: 'https://doi.org/10.1145/3696348.3696875'

target:
    short: HotNets
    full: 'Proceedings of the 23&hairsp;<sup>rd</sup> ACM Workshop on Hot Topics in Networks, 2024'
    link: 'https://conferences.sigcomm.org/hotnets/2024/'

links:
    PDF: '%BASE_URL%/assets/pdf/hotnets24_end_to_end.pdf'
    Slides: 'https://1drv.ms/p/c/40b7196834f13e16/EbH5CrIvV_9Ju7j0a98zNW0Bv3zljE77GsT_6mXoJnTupg?e=1IyH7f'

---

#### Abstract

We propose a performance analysis tool for learning-enabled systems that allows operators to uncover potential performance issues \emph{before} deploying DNNs in their systems. The tools that exist for this purpose require operators to faithfully model all components (a white-box approach) or do inefficient black-box local search. We propose a gray-box alternative, which eliminates the need to precisely model all the system's components. Our approach is faster and finds substantially worse scenarios compared to prior work. We show that a state-of-the-art learning-enabled traffic engineering pipeline can underperform the optimal by $6\times$ --- a much higher number compared to what the authors found.

{% include common_links.md %}

#### BibTeX Citation

```bibtex {% raw %}
@inproceedings{10.1145/3696348.3696875,
author = {Namyar, Pooria and
          Schapira, Michael and
          Govindan, Ramesh and
          Segarra, Santiago and
          Beckett, Ryan and
          Kakarla, Siva Kesava Reddy and
          Arzani, Behnaz},
title = {End-to-End Performance Analysis of Learning-enabled Systems},
year = {2024},
isbn = {9798400712722},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3696348.3696875},
doi = {10.1145/3696348.3696875},
booktitle = {Proceedings of the 23rd ACM Workshop on Hot Topics in Networks},
pages = {86–94},
numpages = {9},
keywords = {Machine Learning for Systems, Performance Analysis},
location = {Irvine, CA, USA},
series = {HotNets '24}
}
{% endraw %} ```

