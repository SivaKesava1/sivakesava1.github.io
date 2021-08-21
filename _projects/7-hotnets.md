---
layout: post
title: "How Complex is DNS?"
categories: [project]
sorter: 7
authors : ['Siva Kesava Reddy Kakarla', '[Ryan Beckett]', '[Todd Millstein]', '[George Varghese]']

year: 2021

# DOI:
#     target: ACM DL
#     link: 'https://doi.org/10.1145/3452296.3472925'

# artifact_badges: ['acm_available', 'acm_functional']

target:
    short: HotNets
    full: 'Twentieth ACM Workshop on Hot Topics in Networks'
    link: 'https://conferences.sigcomm.org/hotnets/2021/'

links:
    # PDF: '%BASE_URL%/assets/pdf/sigcomm21_campion.pdf'
    # Poster: '/assets/pdf/Poster2019.pdf'
    # Tool: 'https://github.com/atang42/batfish/tree/rm-localize'
    # Talk: 'https://youtu.be/CV_-MH7tSLM'
    # Slides: 'https://1drv.ms/p/s!AhY-8TRoGbdAiU5qIyG494E4UfkS?e=0QqV8b'

---

#### Abstract

Motivated by recent results that show that Internet protocols
can be surprisingly complex and, in particular, that BGP is
Turing complete, we ask the same question for the Domain
Name System (DNS). DNS is at least as pervasive and essential as BGP in the global Internet infrastructure. Besides the
scientific interest, the complexity of DNS can have implications for new applications (that can utilize the unsuspected
power of DNS), for security (to understand how attackers can
exploit DNS via new vectors and how to defend against it),
and for verification (to understand basic complexity limits
and suggest new verification algorithms). In this paper, we
show that using the power of $\mathtt{DNAME}$ records, DNS can express regular languages, pushdown systems, and context-free
languages. The first result can be used to build a system
for controlling domain access (of which parental control is
a special case). The second result shows that verification of
DNS configurations in the presence of arbitrary $\mathtt{DNAME}$ rules
is likely to take the time that is cubic in the number of rules.


{% include common_links.md %}

#### BibTeX Citation

Coming soon!