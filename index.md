---
layout: default
title: Home
---
<main id="main" class="site-main">

<h1 class="title-small-caps">About Me</h1>

<div class="bio" markdown="1">
I am a fifth year PhD candidate, in the [CS department][CS@UCLA] at [UCLA], where I am fortunate to be advised by two amazing people, [Prof. Todd Millstein][Todd Millstein] and [Prof. George Varghese][George Varghese]. I have background in networks, formal methods, and programming languages. I am interested in researching all aspects of the design and implementation of high-performance network automation tools with potential future applications to distributed systems. My approach combines insights from verification, testing, anomaly detection, algorithms, and automata theory.

I worked on finding network (router) misconfigurations by automatic template inference
that resulted in a tool called [<span class='small-caps'>SelfStarter</span>]({{ site.baseurl }}/projects/4-selfstarter) that was used in Microsoft. My current focus is on using formal methods to improve the robustness of DNS.
My work, [<span class='small-caps'>GRoot</span>: Proactive Verification of DNS Configurations]({{ site.baseurl }}/projects/5-groot), received a [**SIGCOMM best student paper award**](http://www.sigcomm.org/awards/student-award-recipients) and was featured on the [**APNIC blog**](https://blog.apnic.net/2020/10/29/find-bugs-in-your-dns-zone-files-before-deployment/).

The recent work, [<span class='small-caps'>SCALE</span>:  Automatically Finding RFC Compliance Bugs in DNS Nameservers]({{ site.baseurl }}/projects/8-ferret) found a critical vulnerability in Bind where an attacker with little effort could [**crash**](https://kb.isc.org/v1/docs/cve-2021-25215) Bind nameservers and resolvers remotely. <span class='small-caps'>SCALE</span> was invited for an article in the [USENIX <tt>;login:</tt> magazine](https://www.usenix.org/publications/loginonline/ferret-automatically-finding-rfc-compliance-bugs-dns-nameservers). DNS-OARC [tweeted](https://twitter.com/dnsoarc/status/1390497128825376770)  about the tool saying — “Incredible reception from the audience on @SivaKesavaRK presentation. The automation tool received great compliments from the DNS experts”

{% comment -%}
My research interests lie at the intersection of Networks and Programming Languages.
<!-- My work is focused on addressing two key limitations in the current network verification technology - the lack of formal specifications, and a shallow application that is limited only to the routing layer.  -->
My work is focused on addressing the limitations in the current network verification technology - the lack of formal specifications, and a shallow application that is limited only to the routing layer.
My research seeks to make it easier for operators to design, build, and maintain reliable distributed networks
{%- endcomment -%}

{% comment -%}
My projects in network verification have been in collaboration with [Ryan Beckett], [Behnaz Arzani] and [Karthick Jayaraman] from Microsoft. Our work, [<span class='small-caps'>GRoot</span>: Proactive Verification of DNS Configurations]({{ site.baseurl }}/projects/5-groot), received a [**SIGCOMM best student paper award**](http://www.sigcomm.org/awards/student-award-recipients) and has also been featured on the [**APNIC blog**](https://blog.apnic.net/2020/10/29/find-bugs-in-your-dns-zone-files-before-deployment/).  
{%- endcomment -%}

Before [UCLA] happened, I  was an undergraduate student in the [CSE department][CS@IITKGP] at [IIT Kharagpur] where I was advised by [Prof. Sandip Chakraborty][Sandip Chakraborty] for my undergraduate thesis.

{% include mini_updates.md %}

{% include common_abbrv.md %}

{% include common_links.md %}
</div>



</main>



