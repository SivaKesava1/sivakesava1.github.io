---
layout: post
title: "=sc^GRoot^sc=: Proactive Verification of DNS Configurations"
categories: [project]
sorter: 5
authors : ['Siva Kesava Reddy Kakarla', '[Ryan Beckett]', '[Behnaz Arzani]', '[Todd Millstein]', '[George Varghese]']

year: 2020

DOI:
    target: ACM DL
    link: 'https://doi.org/10.1145/3387514.3405871'

artifact_badges: ['acm_available', 'acm_functional']

awards:
  - icon: star
    desc: 'Best Student Paper Award'

target:
    short: SIGCOMM
    full: 'Proceedings of the ACM Special Interest Group on Data Communication, 2020'
    link: 'https://conferences.sigcomm.org/sigcomm/2020/'

links:
    PDF: '%BASE_URL%/assets/pdf/sigcomm20_groot.pdf'
    # Poster: '/assets/pdf/Poster2019.pdf'
    Tool: 'https://github.com/dns-groot/groot'
    Talk: 'https://youtu.be/CV_-MH7tSLM'
    Slides: 'https://1drv.ms/p/s!AhY-8TRoGbdAiU5qIyG494E4UfkS?e=0QqV8b'

long:
    Slides: 'https://1drv.ms/p/s!AhY-8TRoGbdAiUuCYjFZx3mUoPCG?e=6As6rq'
    Talk: 'https://dl.acm.org/doi/abs/10.1145/3387514.3405871#sec-supp'

---

#### Note

We have updated the paper to handle empty non-terminals as per the RFCs properly. The updated paper is available through the above PDF link.

#### Abstract

The Domain Name System (DNS) plays a vital role in today’s Internet but relies on complex distributed management of host records. DNS
misconfiguration related outages have rendered popular services
like GitHub, HBO, LinkedIn, and Azure inaccessible for extended periods. 
This paper introduces =sc^GRoot^sc=, the first verifier that performs static analysis of DNS configuration files enabling _proactive_ and _exhaustive_
checking for common DNS bugs; by contrast, existing solutions
are _reactive_ and _incomplete_. =sc^GRoot^sc= uses a new, fast verification
algorithm based on generating and enumerating DNS query _equivalence classes_. =sc^GRoot^sc= symbolically executes the set of queries in each
equivalence class to efficiently find (or prove the absence of) any
bugs such as rewrite loops. To prove the correctness of our approach, we develop a formal semantic model of DNS
resolution. Applied to the configuration files from
a campus network with over a hundred thousand records,
=sc^GRoot^sc=  revealed 109 bugs within seconds. When
applied to internal zone files consisting of over $3.5$ million records
from a large infrastructure service provider, =sc^GRoot^sc=  revealed around $160k$ issues of
blackholing, initiating a cleanup. Finally,
on a synthetic dataset with over $65$ million real records,
we find GRoot can scale to networks with tens of millions of
records.

{% include common_links.md %}

#### BibTeX Citation

```bibtex {% raw %}
@inproceedings{10.1145/3387514.3405871,
    author = {Kakarla, Siva Kesava Reddy and 
              Beckett, Ryan and
              Arzani, Behnaz and
              Millstein, Todd and
              Varghese, George},
    title = {GRoot: Proactive Verification of DNS Configurations},
    year = {2020},
    isbn = {9781450379557},
    publisher = {Association for Computing Machinery},
    address = {New York, NY, USA},
    url = {https://doi.org/10.1145/3387514.3405871},
    doi = {10.1145/3387514.3405871},
    booktitle = {Proceedings of the Annual Conference of the ACM Special Interest Group on Data Communication on the Applications, Technologies, Architectures, and Protocols for Computer Communication},
    pages = {310–328},
    numpages = {19},
    keywords = {Static Analysis, Verification, DNS, Formal Methods},
    location = {Virtual Event, USA},
    series = {SIGCOMM ’20}
}
{% endraw %} ```

