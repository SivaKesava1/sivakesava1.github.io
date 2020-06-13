---
layout: post
title: "Does QUIC Kill Your Data Plan? A View Using YouTube Adaptive Streaming Clients"
categories: [project]
sorter: 1
authors : '-- Undergraduate Thesis Work under [Sandip Chakraborty]'

year: 2017

# DOI:
#     target: arXiv
#     link: https://arxiv.org/abs/1902.09033

target:
    short: UG Thesis

links:
    PDF: '%BASE_URL%/assets/pdf/UG_thesis.pdf'
---

#### Abstract

Adaptive bitrate video streaming over the Internet typically uses HTTP over TCP. Lately Quick UDP Internet Connection (QUIC) protocol, introduced by Google, has been shown to improve web browsing performance over TCP. Engineered to have better connection establishment, congestion control, and stream multiplexing capabilities, QUIC seems to be an obvious candidate for replacing TCP for video streaming over the web. In this work, we focus on comparing adaptive bitrate streaming performance over QUIC and TCP. Our experimental analysis is based on $175$ YouTube video streams that are accessed from a browser, and over a controlled network setup such that impact of different parameters can be studied. We observe that QUIC is better in maintaining a higher bitrate during playback, as well as, reduces bitrate switching, relative to TCP. However, QUIC uses more bandwidth to download higher data volume for buffering, especially at low bandwidth, and even suffers from more rebuffering events during playback compared to the use of TCP.

{% include common_links.md %}