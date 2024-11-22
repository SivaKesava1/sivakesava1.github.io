---
layout: post
title: "Towards Safer Heuristics With $\\mathcal{X}$plain"
categories: [project]
sorter: 15
authors : ['[Pantea Karimi]', '[Solal Pirelli]',  Siva Kesava Reddy Kakarla, '[Ryan Beckett]', '[Santiago Segarra]', '[Beibin Li]', '[Pooria Namyar]', '[Behnaz Arzani]']

year: 2024

DOI:
    target: ACM DL
    link: 'https://doi.org/10.1145/3696348.3696884'

target:
    short: HotNets
    full: 'Proceedings of the 23&hairsp;<sup>rd</sup> ACM Workshop on Hot Topics in Networks, 2024'
    link: 'https://conferences.sigcomm.org/hotnets/2024/'

links:
    PDF: '%BASE_URL%/assets/pdf/hotnets24_xplain.pdf'
    Slides: 'https://1drv.ms/p/c/40b7196834f13e16/EUAvMJkprYhMqmn6YImVT7oBqEVxMLrfLbcVNZB1-XMRGg?e=E1qsVW&nav=eyJzSWQiOjM3NSwiY0lkIjozMzg1MDgwMDU2fQ'

---

#### Abstract

Many problems that cloud operators solve are computationally expensive, and operators often use heuristic algorithms (that are faster and scale better than optimal) to solve them more efficiently.
Heuristic analyzers enable operators to find when and by how much their heuristics underperform. However, these tools do not provide enough detail for operators to mitigate the heuristic's impact in practice: they only discover a _single input instance_ that causes the heuristic to underperform (and not the full set) and they do not _explain why_.

We propose $\mathcal{X}$Plain, a tool that extends these analyzers and helps operators understand when and why their heuristics underperform. 
We present promising initial results that show such an extension is viable. 

{% include common_links.md %}

#### BibTeX Citation

```bibtex {% raw %}
@inproceedings{10.1145/3696348.3696884,
author = {Karimi, Pantea and
          Pirelli, Solal and
          Kakarla, Siva Kesava Reddy and
          Beckett, Ryan and
          Segarra, Santiago and
          Li, Beibin and
          Namyar, Pooria and
          Arzani, Behnaz},
title = {Towards Safer Heuristics With XPlain},
year = {2024},
isbn = {9798400712722},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3696348.3696884},
doi = {10.1145/3696348.3696884},
booktitle = {Proceedings of the 23rd ACM Workshop on Hot Topics in Networks},
pages = {68–76},
numpages = {9},
keywords = {Domain-Specific Language, Explainable Analysis, Heuristic Analysis},
location = {Irvine, CA, USA},
series = {HotNets '24}
}
{% endraw %} ```

