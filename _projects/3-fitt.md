---
layout: post
title: "Expect More from the Networking: DDoS Mitigation by =sc^FITT^sc= in Named Data Networking"
categories: [project]
sorter: 3
preprint: https://arxiv.org/abs/1902.09033
authors : ['[Zhiyi Zhang]', '[Vishrant Vasavada]', 'Siva Kesava Reddy Kakarla', '[Eric Osterweil]', '[Lixia Zhang]']

year: 2019
month: Feb

DOI:
    target: arXiv
    link: https://arxiv.org/abs/1902.09033

target:
    short: arXiv

links:
    PDF: '%BASE_URL%/assets/pdf/FITT.pdf'
---

#### Abstract

Distributed Denial of Service (DDoS) attacks have plagued the Internet for decades, but defenses have not fundamentally outpaced attackers. Instead, the size and rate of growth in attacks have actually outpaced carriers’ and DDoS mitigation services’ growth. In this paper, we comprehensively examine ways in which Named Data Networking (NDN), a proposed data-centric Internet architecture, fundamentally addresses some of the principle weaknesses in today’s DDoS defenses in IP networking. We argue that NDN’s architectural changes (even when incrementally deployed) can make DDoS attacks fundamentally more difficult to launch and less effective.

We present a new DDoS mitigation solution – Finegrained Interest Traffic Throttling _=sc^FITT^sc=_, to leverage NDN’s features to combat DDoS in the Internet of Things (IoT) age. =sc^FITT^sc= enables _the network_ to detect DDoS directly from feedback from victims, throttle DDoS traffic along its exact path in the network, and perform reinforcement control over the misbehaving entities _at their sources_. In cases like the Mirai attacks, where smart IoT devices (smart cameras, refrigerators, etc.) were able to cripple high-capacity service providers using diverse DDoS Tactics Techniques and Procedures (TTPs), =sc^FITT^sc= would be able to precisely squelch the attack traffic at its distributed sources, without disrupting other legitimate application traffic running on the same devices. =sc^FITT^sc= offers an incrementally deployable solution for service providers to effectuate the application-level remediation at the sources, which remains unattainable in today’s DDoS market. Our extensive simulations results show that =sc^FITT^sc= can effectively throttle attack traffic in a short time and
achieve over 99% legitimate traffic.

#### BibTeX Citation

```bibtex {% raw %}
@article{DBLP:journals/corr/abs-1902-09033,
  author    = {Zhiyi Zhang and
               Vishrant Vasavada and
               Siva Kesava Reddy K. and
               Eric Osterweil and
               Lixia Zhang},
  title     = {Expect More from the Networking: DDoS Mitigation by {FITT} in Named
               Data Networking},
  journal   = {CoRR},
  volume    = {abs/1902.09033},
  year      = {2019},
  url       = {http://arxiv.org/abs/1902.09033},
  archivePrefix = {arXiv},
  eprint    = {1902.09033},
  timestamp = {Tue, 21 May 2019 18:03:38 +0200},
  biburl    = {https://dblp.org/rec/journals/corr/abs-1902-09033.bib},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
{% endraw %} ```

{% include common_links.md %}