---
layout: post
title: "Rethinking Machine Learning Collective Communication as a Multi-Commodity Flow Problem"
categories: [project]
sorter: 9
preprint: https://arxiv.org/abs/2305.13479
authors : ['[Behnaz Arzani]', 'Siva Kesava Reddy Kakarla', '[Miguel Castro]', '[Srikanth Kandula]', '[Saeed Maleki]', '[Luke Marshall]']

year: 2023
month: May

DOI:
    target: arXiv
    link: https://arxiv.org/abs/2305.13479

target:
    short: arXiv

links:
    PDF: '%BASE_URL%/assets/pdf/teccl.pdf'
---

#### Abstract

We show communication schedulers’ recent work proposed for ML collectives does not scale to the increasing problem sizes that arise from training larger models. These works also often produce suboptimal schedules. We make a connection with similar problems in traffic engineering and propose a new method, =sc^TE-CCL^sc=, that finds better uality schedules (_e.g._, finishes collectives faster and/or while sending fewer bytes) and does so more quickly on larger topologies. We present results on many different GPU topologies that show substantial improvement over the state-of-the-art.

#### BibTeX Citation

```bibtex {% raw %}
@misc{arzani2023rethinking,
      title={Rethinking Machine Learning Collective Communication as a Multi-Commodity Flow Problem}, 
      author={Behnaz Arzani and Siva Kesava Reddy Kakarla and Miguel Castro and Srikanth Kandula and Saeed Maleki and Luke Marshall},
      year={2023},
      eprint={2305.13479},
      archivePrefix={arXiv},
      primaryClass={cs.NI}
}
{% endraw %} ```

{% include common_links.md %}