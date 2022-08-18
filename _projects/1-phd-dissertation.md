---
layout: post
title: "Formal Methods for a Robust Domain Name System"
categories: [project]
sorter: 1
authors : ['Siva Kesava Reddy Kakarla']

year: 2022

# DOI:
#     target: arXiv
#     link: https://arxiv.org/abs/1902.09033

target:
    short: PhD Dissertation

links:
    PDF: '%BASE_URL%/assets/pdf/dissertation_phd.pdf'
---

#### Abstract

The Domain Name System (DNS), one of the foundations of the modern-day Internet,
primarily translates domain names into IP addresses, enabling easy access to online services.
DNS name resolution appears simple at a high level but has evolved into a complex and
intricate protocol over time. Errors in either DNS configurations or DNS implementations have far-reaching disruptive consequences. This is evident from past DNS issues that have rendered popular services such as GitHub, Twitter, HBO, LinkedIn, Yelp, and Azure inaccessible for extended periods.
In this dissertation, I describe my work toward making the DNS as robust as possible by combining formal methods with DNS-specific insights to provide strong guarantees.

This dissertation presents the first formalization of DNS semantics, which I developed
from multiple RFCs; this serves as the foundation for the rest of my work.
Second, I detail a new technique, =sc^SCALE^sc=, for finding RFC compliance errors in DNS nameserver implementations via automatic test generation.
=sc^SCALE^sc= symbolically executes the developed DNS formal model to jointly generate both the test queries and configurations (zone files).
Using =sc^SCALE^sc=, I identified $30$ new bugs in $8$ popular open-source DNS implementations such
as =sc^Bind^sc=, =sc^PowerDNS^sc=, =sc^Knot^sc=, and =sc^Nsd^sc=, including $3$ previously unknown critical security vulnerabilities.
Third, I describe =sc^GRoot^sc=, the first verification tool for DNS configurations.
Given the DNS zone files of an organization and a property of interest, =sc^GRoot^sc= automatically verifies that the property holds for all possible DNS queries or provides all counterexamples.
=sc^GRoot^sc= performs exhaustive and proactive static analysis of DNS configuration files using an efficient algorithm for finding the equivalence classes of all possible queries to guarantee key correctness properties.
I conclude with a theoretical analysis of the DNS to categorize its complexity and expressive power.

{% include common_links.md %}


#### BibTeX Citation

```bibtex {% raw %}
@phdthesis{kakarla2022formal,
  title={Formal Methods for a Robust Domain Name System},
  author={Kakarla, Siva Kesava Reddy},
  year={2022},
  school={UCLA}
}
{% endraw %} ```