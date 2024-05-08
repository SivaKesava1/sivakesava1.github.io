---
layout: post
title: "=sc^MESSI^sc=: Behavioral Testing of BGP Implementations"
categories: [project]
sorter: 11
authors : ['Rathin Singha', 'Rajdeep Mondal', '[Ryan Beckett]', 'Siva Kesava Reddy Kakarla', '[Todd Millstein]', '[George Varghese]']

year: 2024

DOI:
    target: USENIX
    link: https://www.usenix.org/conference/nsdi24/presentation/singha

target:
    short: NSDI
    full: 'Proceedings of the 21&hairsp;<sup>st</sup> USENIX Symposium on Networked Systems Design and Implementation, 2024'
    link: 'https://www.usenix.org/conference/nsdi24'

links:
    PDF: '%BASE_URL%/assets/pdf/nsdi24_messi.pdf'
    Tool: 'https://github.com/rsingha108/MESSI'
---


#### Abstract

Complex network protocols like the Border Gateway Protocol (BGP) are prone to implementation errors that cause unintended behaviors with potentially global consequences. We introduce an approach and tool called =sc^MESSI^sc= (Modular Exploration of State and Structure Inclusively) to automatically generate tests for black-box BGP implementations. Our approach is _model-based_, leveraging an executable model of BGP to generate behavioral tests. However, doing so effectively requires addressing new challenges such as the stateful nature of BGP and the need to generate complex structures like regular expressions in route maps. We used =sc^MESSI^sc= to generate roughly $150K$ tests that capture different aspects of BGP, such as route-map filtering, the decision process, route aggregation, and dynamics. These tests identified $22$ correctness bugs across several widely used open-source BGP implementations (FRR, Quagga, GoBGP, BIRD, Batfish) and one closed-source implementation. Eight of these errors have already been fixed. While our models are BGP-specific our approach is not: thus we expect it can be adapted to test other stateful protocols with complex structures.

{% include common_links.md %}


#### BibTeX Citation

```bibtex {% raw %}
@inproceedings {295579,
author = {Rathin Singha and Rajdeep Mondal and Ryan Beckett and Siva Kesava Reddy Kakarla and Todd Millstein and George Varghese},
title = {{MESSI}: Behavioral Testing of {BGP} Implementations},
booktitle = {21st USENIX Symposium on Networked Systems Design and Implementation (NSDI 24)},
year = {2024},
isbn = {978-1-939133-39-7},
address = {Santa Clara, CA},
pages = {1009--1023},
url = {https://www.usenix.org/conference/nsdi24/presentation/singha},
publisher = {USENIX Association},
month = apr
}
{% endraw %} ```
