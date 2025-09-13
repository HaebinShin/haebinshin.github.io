---
permalink: /
title: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi, I’m a graduate student at KAIST, specializing in natural language processing (NLP) and large language models (LLMs), advised by Prof. [Minjoon Seo](https://seominjoon.github.io/). I am also a research intern at [Microsoft Research](https://www.microsoft.com/en-us/research/), where I work with [Yeyun Gong](https://www.microsoft.com/en-us/research/people/yegong/), [Lei Ji](https://www.microsoft.com/en-us/research/people/leiji/), and [Qi Chen](https://www.microsoft.com/en-us/research/people/cheqi/). I was honored with the **Stars of Tomorrow** award at [Microsoft Research Asia](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/). 

Previously, I worked as a research scientist at [Samsung Research](https://research.samsung.com/) and [ESTsoft](https://estsoft.ai/en/), contributing to applied LLM systems for [Galaxy AI](https://www.samsung.com/us/galaxy-ai/). I conducted research on foundation models, primarily on LLM pre-/post-training, information retrieval, and semantic parsing.

My research interests lie in making large language models more *efficient* and *practical*:
- **Efficient** training and inference methods for LLMs, including cost-efficient inference ([NAACL 2025](https://arxiv.org/abs/2411.15927)), distillation ([ICML 2025](https://arxiv.org/abs/2503.19123), [NAACL 2025](https://arxiv.org/abs/2411.15927)), and data mixture optimization ([DynamixSFT](https://arxiv.org/abs/2508.12116))
- **Real-world impact**, advancing agent adaptability ([NAACL 2025](https://arxiv.org/abs/2411.15927)), scientific discovery ([GenBio 2025](https://arxiv.org/abs/2409.19788), [BioNLP 2025](https://aclanthology.org/2025.bionlp-1.21)), and real-time information access ([NAACL 2024](https://arxiv.org/abs/2311.08329)).


# Work Experience
<div class="work-list">
  {% for w in site.data.work %}
    {% include work-item.html
       logo=w.logo company=w.company role=w.role tenure=w.tenure location=w.location %}
  {% endfor %}
</div>


# Selected Publications
<div class="pub-list">
  {% for p in site.data.selected_publications %}
    {% include pub-item.html
       title=p.title
       authors=p.authors_html
       venue=p.venue
       badge=p.badge
       paper_url=p.paper_url
       code_url=p.code_url
       project_url=p.project_url
       dataset_url=p.dataset_url %}
  {% endfor %}
</div>

# Education
<div class="edu-list">
  {% for e in site.data.edu %}
    {% include edu-item.html
      logo="/images/school/kaist.png"
      school=e.school
      degree=e.degree
      dept=e.dept
      period=e.period %}
  {% endfor %}
</div>

# Selected Honors & Awards
<div class="award-list">
  {% for h in site.data.honors %}
    {% include honor-item.html
      title=h.title
      assoc=h.assoc
      desc=h.desc
      date=h.date %}
  {% endfor %}
</div>
 
# Patents
<div class="patent-list">
  {% for pt in site.data.patents %}
    {% include patent-item.html
      title=pt.title
      country=pt.country
      appl_num=pt.appl_num
      filed_yy=pt.filed_yy
      patent_num=pt.patent_num
      granted_yy=pt.granted_yy
      url=pt.url %}
  {% endfor %}
</div>