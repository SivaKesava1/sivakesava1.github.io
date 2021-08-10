---
layout: post
title: "=sc^Campion^sc=: Debugging Router Configuration Differences"
categories: [project]
sorter: 6
authors : ['Alan Tang', 'Siva Kesava Reddy Kakarla', '[Ryan Beckett]', '[Ennan Zhai]','[Matt Brown]', '[Todd Millstein]', '[Yuval Tamir]', '[George Varghese]']

year: 2021

DOI:
    target: ACM DL
    link: 'https://doi.org/10.1145/3452296.3472925'

artifact_badges: ['acm_available', 'acm_functional']

target:
    short: SIGCOMM
    full: 'Proceedings of the ACM Special Interest Group on Data Communication, 2021'
    link: 'https://conferences.sigcomm.org/sigcomm/2021/'

links:
    PDF: '%BASE_URL%/assets/pdf/sigcomm21_campion.pdf'
    # Poster: '/assets/pdf/Poster2019.pdf'
    Tool: 'https://github.com/atang42/batfish/tree/rm-localize'
    # Talk: 'https://youtu.be/CV_-MH7tSLM'
    # Slides: 'https://1drv.ms/p/s!AhY-8TRoGbdAiU5qIyG494E4UfkS?e=0QqV8b'

---

#### Abstract

We present a new approach for debugging two router configurations that are intended to be behaviorally equivalent. Existing router verification techniques cannot identify all differences or localize those differences to relevant configuration lines. Our approach addresses these limitations through a _modular_ analysis, which separately analyzes pairs of corresponding configuration components.
It handles all router components that affect routing and forwarding, including configuration for BGP, OSPF, static routes, route maps and ACLs. Further, for many configuration components our modular approach enables simple _structural equivalence_ checks to be used without additional loss of precision versus modular semantic checks, aiding both efficiency and error localization. We implemented this approach in the tool =sc^Campion^sc= and applied it to 
debugging pairs of backup routers from different manufacturers and validating replacement of critical routers.
=sc^Campion^sc= analyzed 30 proposed router replacements in a production cloud network and proactively detected four configuration bugs, including a route reflector bug that could have caused a severe outage.
=sc^Campion^sc= also found multiple differences between backup routers from different vendors in a university network. These were undetected for three years, and depended on subtle semantic differences that the operators said they were "highly unlikely" to detect by "just eyeballing the configs."

{% include common_links.md %}

#### BibTeX Citation

```bibtex {% raw %}
@inproceedings{10.1145/3452296.3472925,
    author = {Tang, Alan and
              Kakarla, Siva Kesava Reddy and
              Beckett, Ryan and
              Zhai, Ennan and
              Brown, Matt and
              Millstein, Todd and
              Tamir, Yuval and
              Varghese, George},
    title = {Campion: Debugging Router Configuration Differences},
    year = {2021},
    isbn = {9781450383837},
    publisher = {Association for Computing Machinery},
    address = {New York, NY, USA},
    url = {https://doi.org/10.1145/3452296.3472925},
    doi = {10.1145/3452296.3472925},
    booktitle = {Proceedings of the 2021 ACM SIGCOMM 2021 Conference},
    pages = {748–761},
    numpages = {14},
    keywords = {error localization, network verification, modular reasoning, equivalence checking},
    location = {Virtual Event, USA},
    series = {SIGCOMM '21}
}
{% endraw %} ```