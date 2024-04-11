---
layout: post
title: "=sc^SCALE^sc=: Automatically Finding RFC Compliance Bugs in DNS Nameservers"
categories: [project]
sorter: 8
authors : ['Siva Kesava Reddy Kakarla', '[Ryan Beckett]', '[Todd Millstein]', '[George Varghese]']

year: 2022

awards:
  - icon: star
    desc: 'IRTF/IETF Applied Networking Research Prize'

DOI:
    target: USENIX
    link: https://www.usenix.org/conference/nsdi22/presentation/kakarla

target:
    short: NSDI
    full: 'Proceedings of the 19&hairsp;<sup>th</sup> USENIX Symposium on Networked Systems Design and Implementation, 2022'
    link: 'https://www.usenix.org/conference/nsdi22'

links:
    PDF: '%BASE_URL%/assets/pdf/nsdi22_ferret.pdf'
    Tool: 'https://github.com/dns-groot/Ferret'
    Slides: 'https://1drv.ms/p/s!AhY-8TRoGbdAiWrBUlFjQscCZMsE?e=kJjbce'
    Talk: 'https://www.youtube.com/watch?v=LIK7p2I4ZlI'
---


#### Abstract

The Domain Name System (DNS) has intricate features that interact in subtle ways. Bugs in DNS implementations can lead to incorrect or implementation-dependent behavior, security vulnerabilities, and more. We introduce the first approach for finding RFC compliance errors in DNS nameserver implementations, via automatic test generation. Our =sc^SCALE^sc= (Small-scope Constraint-driven Automated Logical Execution) approach _jointly_ generates zone files and corresponding queries to cover RFC behaviors specified by an executable model of DNS resolution. We have built a tool called =sc^Ferret^sc= based on this approach and applied it to test $8$ open-source DNS implementations, including popular implementations such as Bind, PowerDNS, Knot, and Nsd. =sc^Ferret^sc= generated over $13.5K$ test files, of which $62\%$ resulted in some difference among implementations. We identified and reported $30$ new unique bugs from these failed test cases, including at least one bug in every implementation, of which $20$ have already been fixed. Many of these existed in even the most popular DNS implementations, including a new critical vulnerability in Bind that attackers could easily exploit to crash DNS resolvers and nameservers remotely.

{% include common_links.md %}


#### BibTeX Citation

```bibtex {% raw %}
@inproceedings {278336,
author = {Siva Kesava Reddy Kakarla and Ryan Beckett and Todd Millstein and George Varghese},
title = {{SCALE}: Automatically Finding {RFC} Compliance Bugs in {DNS} Nameservers},
booktitle = {19th USENIX Symposium on Networked Systems Design and Implementation (NSDI 22)},
year = {2022},
isbn = {978-1-939133-27-4},
address = {Renton, WA},
pages = {307--323},
url = {https://www.usenix.org/conference/nsdi22/presentation/kakarla},
publisher = {USENIX Association},
month = apr,
}
{% endraw %} ```

