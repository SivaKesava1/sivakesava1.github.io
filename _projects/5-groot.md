---
layout: post
title: "GRoot: Proactive Verification of DNS Configurations"
categories: [project]
sorter: 5
authors : ['Siva Kesava Reddy Kakarla', '[Ryan Beckett]', '[Behnaz Arzani]', '[Todd Millstein]', '[George Varghese]']

year: 2020

# DOI:
#     target: ACM DL

target:
    short: SIGCOMM
    full: 'Proceedings of the ACM Special Interest Group on Data Communication, 2020'
    link: 'https://conferences.sigcomm.org/sigcomm/2020/'

links:
    PDF: '%BASE_URL%/assets/pdf/nsdi20_selfstarter.pdf'
    Tool: 'https://github.com/dns-groot/groot'
    Poster: /assets/pdf/Poster2019.pdf
---

#### Abstract

The Domain Name System (DNS) plays a vital role in today’s Internet but relies on complex distributed management of host records.
DNS misconfigurations are responsible for many outages that have
rendered popular services such as GitHub, Twitter, HBO, LinkedIn,
Yelp, and Azure inaccessible for extended periods of time. This
paper introduces GRoot, the first verifier that performs static analysis of DNS configuration files enabling _proactive_ and _exhaustive_
checking for common DNS bugs; by contrast, existing solutions
are _reactive_ and _incomplete_. GRoot uses a new, fast verification
algorithm based on generating and enumerating DNS query _equivalence classes_. GRoot symbolically executes the set of queries in each
equivalence class to efficiently find (or prove the absence of) any
bugs such as rewrite loops or no response. To prove the correctness of our approach, we develop a formal semantic model of DNS
resolution. Applied to a set of configuration files obtained from
a large campus network with over a hundred thousand records,
GRoot revealed 111 bugs, analyzing the network in seconds. When
applied to internal zone files consisting of over $3.5$ million records
from a large CDN provider, GRoot revealed around $160k$ issues of
blackholing, which initiated a clean up of the zone files. Finally,
on a synthetic dataset created from over $65$ million real records,
we find that GRoot can scale to networks with tens of millions of
records.

{% include common_links.md %}