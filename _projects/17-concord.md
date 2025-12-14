---
layout: post
title: "=sc^Concord^sc=: Learning Network Configuration Contracts"
categories: [project]
sorter: 16
authors : ['[Ryan Beckett]', '[Francis Y. Yan]', Raghunadha Reddy Pocha, Vineesh V. Raj, Ayyub Shaik, 'Siva Kesava Reddy Kakarla']

year: 2026

DOI:
    target: ACM DL
    link: 'https://doi.org/10.1145/3767295.3769338'

target:
    short: EUROSYS
    full: '21st European Conference on Computer Systems (EUROSYS ''26)'
    link: 'https://2026.eurosys.org/'


links:
    PDF: '%BASE_URL%/assets/pdf/eurosys26_concord.pdf'

    
---

#### Abstract

Misconfiguration is frequently cited as a leading cause of service disruptions and outages. To prevent misconfiguration, we introduce network _contracts_---lightweight configuration checks that run efficiently, localize errors to specific lines, and require no heavyweight modeling of network protocols. We develop a tool =sc^Concord^sc= to learn contracts automatically from example network configurations. By checking these learned contracts against new or changed configurations, =sc^Concord^sc= finds likely configuration bugs before they can impact the network. Key to our approach is a scalable algorithm for learning "relational" contracts that capture complex dependencies between configuration settings. We deployed =sc^Concord^sc= as part of a cloud-based configuration management service and evaluated its scalability, coverage, precision, and utility on two large real-world configuration datasets.

{% include common_links.md %}

#### BibTeX Citation

Coming soon!

