---
layout: post
title: "IEEE 802.11ac DBCA: A Tug of War between Channel Utilization and Fairness"
categories: [project]
sorter: 2
IEEE: https://ieeexplore.ieee.org/document/8254448
authors : ['[Saketh Mahankali]', 'Siva Kesava Reddy Kakarla',  'Raja Karmakar',  'Samiran Chattopadhyay', '[Sandip Chakraborty]']

year: 2017

DOI:
    target: IEEE
    link: https://doi.org/10.1109/GLOCOM.2017.8254448

target:
    short: GLOBECOM
    full: 'Proceedings of the IEEE Global Communications Conference, 2017'
    link: 'https://globecom2017.ieee-globecom.org/'

links:
    PDF: '%BASE_URL%/assets/pdf/globecom17.pdf'
---

#### Abstract

IEEE 802.11ac supports _Dynamic Bandwidth Channel Access_ (DBCA), where a wireless station dynamically selects the channel bandwidth based on the availability of the secondary channels. Although DBCA reduces the possibility of starvation due to non-availability of secondary channels, however, to the best of our knowledge, no existing works look into the performance benefits of IEEE 802.11ac DBCA based on theoretical modeling. In this paper, we develop a two dimensional Markov chain approach to model the performance of DBCA under various channel bonding conditions. We validate the proposed model based on a real testbed implementation. From the thorough analysis of the numerical results obtained from the model, we show that although DBCA improves channel utilization for secondary channels, it requires proper channel allocations and bonding level distributions across the wireless channels for reducing unfairness in the network. We observe that under certain circumstances, the secondary channel users can affect the throughput of primary channel users, which may introduce a short-term unfairness and a significant performance drop in the network.

#### BibTeX Citation

```bibtex {% raw %}
@inproceedings{DBLP:conf/globecom/MahankaliKKCC17,
  author    = {Saketh Mahankali and
               Siva Kesava Reddy K. and
               Raja Karmakar and
               Samiran Chattopadhyay and
               Sandip Chakraborty},
  title     = {{IEEE} 802.11ac {DBCA:} {A} Tug of War between Channel Utilization
               and Fairness},
  booktitle = {2017 {IEEE} Global Communications Conference, {GLOBECOM} 2017, Singapore,
               December 4-8, 2017},
  pages     = {1--6},
  publisher = {{IEEE}},
  year      = {2017},
  url       = {https://doi.org/10.1109/GLOCOM.2017.8254448},
  doi       = {10.1109/GLOCOM.2017.8254448},
  timestamp = {Wed, 16 Oct 2019 14:14:51 +0200},
  biburl    = {https://dblp.org/rec/conf/globecom/MahankaliKKCC17.bib},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
{% endraw %} ```


{% include common_links.md %}