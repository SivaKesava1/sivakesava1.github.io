---
layout: post
title: "=sc^Campion^sc=: Debugging Router Configuration Differences"
categories: [project]
sorter: 6
authors : ['Alan Tang', 'Siva Kesava Reddy Kakarla', '[Ryan Beckett]', '[Ennan Zhai]','[Matt Brown]', '[Todd Millstein]', '[Yuval Tamir]', '[George Varghese]']

year: 2021

target:
    short: SIGCOMM
    full: 'Proceedings of the ACM Special Interest Group on Data Communication, 2021'
    link: 'https://conferences.sigcomm.org/sigcomm/2021/'

---

#### Abstract

We present a new approach for debugging two router configurations that are intended to be behaviorally equivalent. Existing router verification techniques cannot identify all differences or localize those differences to relevant configuration lines. Our approach addresses these limitations through a _modular_ analysis, which separately analyzes pairs of corresponding configuration components.
It handles all router components that affect routing and forwarding, including configuration for BGP, OSPF, static routes, route maps and ACLs. Further, for many configuration components our modular approach enables simple _structural equivalence_ checks to be used without loss of precision, aiding both efficiency and error localization. We implemented this approach in the tool =sc^Campion^sc= and applied it to 
debugging pairs of backup routers from different manufacturers and validating replacement of critical routers.
=sc^Campion^sc= analyzed $30$ proposed router replacements in a production cloud network and proactively detected four configuration bugs, including a route reflector bug that could have caused a severe outage.
=sc^Campion^sc= also found multiple differences between backup routers from different vendors in a university network. These were undetected for three years, and depended on subtle semantic differences that the operators said they were "highly unlikely" to detect by "just eyeballing the configs."

{% include common_links.md %}

