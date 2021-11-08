---
layout: post
title: "How Complex is DNS?"
categories: [project]
sorter: 7
authors : ['Siva Kesava Reddy Kakarla', '[Ryan Beckett]', '[Todd Millstein]', '[George Varghese]']

year: 2021

DOI:
    target: ACM DL
    link: 'https://doi.org/10.1145/3484266.3487369'

target:
    short: HotNets
    full: 'Proceedings of the 20&hairsp;<sup>th</sup> ACM Workshop on Hot Topics in Networks, 2021'
    link: 'https://conferences.sigcomm.org/hotnets/2021/'

links:
    PDF: '%BASE_URL%/assets/pdf/hotnets21_complexity.pdf'
    Talk: 'https://www.youtube.com/watch?v=oylZ5pknAZc'
    Slides: 'https://1drv.ms/p/s!AhY-8TRoGbdAiVaMkrSzUzuakZzE?e=iuugNs'

---

#### Abstract

Motivated by recent results that show that Internet protocols
can be surprisingly complex and, in particular, that BGP is
Turing complete, we ask the same question for the Domain
Name System (DNS). DNS is at least as pervasive and essential as BGP in the global Internet infrastructure. Besides the
scientific interest, the complexity of DNS can have implications for new applications (that can utilize the unsuspected
power of DNS),
and for verification (to understand basic complexity limits
and suggest new verification algorithms). In this paper, we
show that using the power of $\mathtt{DNAME}$ records, DNS can express regular languages and pushdown systems. The first result can be used to build a system
for controlling domain access (of which parental control is
a special case). The second result shows that verification of
DNS zone files is likely to take time that is at least cubic in
the number of records.



{% include common_links.md %}

#### BibTeX Citation

```bibtex {% raw %}
@inproceedings{10.1145/3484266.3487369,
author = {Kakarla, Siva Kesava Reddy and Beckett, Ryan and Millstein, Todd and Varghese, George},
title = {How Complex is DNS?},
year = {2021},
isbn = {9781450390873},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3484266.3487369},
doi = {10.1145/3484266.3487369},
booktitle = {Proceedings of the Twentieth ACM Workshop on Hot Topics in Networks},
pages = {116–122},
numpages = {7},
keywords = {verification complexity, automata theory, DNS, pushdown systems, computational complexity},
location = {Virtual Event, United Kingdom},
series = {HotNets '21}
}
{% endraw %} ```