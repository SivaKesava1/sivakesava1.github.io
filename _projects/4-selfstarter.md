---
layout: post
title: "=sc^SelfStarter^sc=: Finding Network Misconfigurations by Automatic Template Inference"
categories: [project]
sorter: 4
authors : ['Siva Kesava Reddy Kakarla', 'Alan Tang', '[Ryan Beckett]', '[Karthick Jayaraman]', '[Todd Millstein]', '[Yuval Tamir]', '[George Varghese]']

year: 2020

DOI:
    target: USENIX
    link: https://www.usenix.org/conference/nsdi20/presentation/kakarla

target:
    short: NSDI
    full: 'Proceedings of the 17&hairsp;<sup>th</sup> USENIX Symposium on Networked Systems Design and Implementation, 2020'
    link: 'https://www.usenix.org/conference/nsdi20'

links:
    PDF: '%BASE_URL%/assets/pdf/nsdi20_selfstarter.pdf'
    Tool: 'https://github.com/SivaKesava1/SelfStarter'
    Slides: 'https://1drv.ms/p/s!AhY-8TRoGbdAiGUEzxNIj69-BVJy?e=m00tIw'
    Talk: 'https://www.youtube.com/watch?v=X4tk4w_PEv0'
---


#### Abstract

Network verification to detect router configuration errors typically requires an explicit correctness _specification_.  Unfortunately, specifications often either do not exist, are incomplete, or are written informally in English. We describe an approach to infer likely network configuration errors without a specification through a form of automated _outlier detection_. Unlike prior techniques, our approach can identify outliers even for complex, structured configuration elements that have a variety of intentional differences across nodes, like access-control lists, prefix lists, and route policies.  

Given a collection of configuration elements, our approach automatically infers a set of parameterized _templates_, modeling the (likely) intentional differences as variations within a template while modeling the (likely) erroneous differences as variations across templates. We have implemented our algorithm, which we call _structured generalization_, in a tool called =sc^SelfStarter^sc= and used it to automatically identify configuration outliers in a collection of datacenter networks from a large cloud provider, the wide-area network from the same cloud provider, and the campus network of a large university. =sc^SelfStarter^sc= found misconfigurations in all three networks, including $43$ previously unknown bugs, and is in the process of adoption in the configuration management system of a major cloud provider. 

{% include common_links.md %}


#### BibTeX Citation

```bibtex {% raw %}
@inproceedings {246314,
    author = {Siva Kesava Reddy Kakarla and
              Alan Tang and
              Ryan Beckett and
              Karthick Jayaraman and
              Todd Millstein and
              Yuval Tamir and
              George Varghese},
    title = {Finding Network Misconfigurations by Automatic Template Inference },
    booktitle = {17th {USENIX} Symposium on Networked Systems Design and Implementation ({NSDI} 20)},
    year = {2020},
    isbn = {978-1-939133-13-7},
    address = {Santa Clara, CA},
    pages = {999--1013},
    url = {https://www.usenix.org/conference/nsdi20/presentation/kakarla},
    publisher = {{USENIX} Association},
    month = feb,
}
{% endraw %} ```

