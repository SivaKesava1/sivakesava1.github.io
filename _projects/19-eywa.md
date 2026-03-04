---
layout: post
title: "=sc^Eywa^sc=: Automating Model Based Testing using LLMs"
categories: [project]
sorter: 19
authors : ['Rajdeep Mondal', 'Rathin Singha', '[Todd Millstein]', '[George Varghese]', '[Ryan Beckett]', 'Siva Kesava Reddy Kakarla']

year: 2026

# DOI:
#     target: USENIX
#     link: 

target:
    short: NSDI
    full: 'Proceedings of the 23&hairsp;<sup>rd</sup> USENIX Symposium on Networked Systems Design and Implementation, 2026'
    link: 'https://www.usenix.org/conference/nsdi26'

artifact_badges: ['usenix_available', 'usenix_functional', 'usenix_reproduced']

links:
    PDF: '%BASE_URL%/assets/pdf/nsdi26_eywa.pdf'
    Tool: 'https://github.com/microsoft/Model_Based_Testing_Using_LLMs'
    # Slides: 
    # Talk:
---


#### Abstract

Model-based testing (MBT), whereby a model of the system under test is analyzed to generate high-coverage test cases, has been used to test protocol implementations. A key barrier to the use of MBT is the need for users to understand protocol RFCs in detail to create a compliant model.

Our new approach to MBT uses LLMs to automatically build rich models of intended protocol behavior from knowledge embedded in Request for Comments documents (RFCs), blogs, and other natural language sources. Our approach addresses key challenges with using LLMs, including hallucinations and their inability to monolithically generate complex protocol models. We realize our approach through a novel protocol testing framework =sc^Eywa^sc=, and demonstrate its effectiveness through extensive case studies of DNS and BGP, and a smaller study of SMTP. Despite minimal user effort, applying =sc^Eywa^sc= enabled the discovery of 33 unique bugs across widely used DNS, BGP, and SMTP implementations, 16 of which were previously undiscovered despite extensive prior testing with manually crafted models.

{% include common_links.md %}


#### BibTeX Citation

Coming soon!
