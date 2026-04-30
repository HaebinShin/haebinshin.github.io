---
permalink: /
title: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi, I’m an incoming PhD student at the [University of Michigan](https://umich.edu/), co-advised by Prof. [Lu Wang](https://web.eecs.umich.edu/~wangluxy/) and Prof. [Honglak Lee](https://web.eecs.umich.edu/~honglak/). I earned my MS from KAIST advised by Prof. [Minjoon Seo](https://seominjoon.github.io/). My research focuses on making large language models (LLMs) more efficient and reliable, with a particular interest in how they acquire and utilize knowledge under real-world constraints.

Previously, I spent eight years in industry as a research scientist at [Samsung Research](https://research.samsung.com/) and [ESTsoft](https://estsoft.ai/en/), where I worked on applied LLM systems including [Galaxy AI](https://www.samsung.com/us/galaxy-ai/), with a focus on LLM pre-/post-training, information retrieval, and semantic parsing. I also interned at [Microsoft Research](https://www.microsoft.com/en-us/research/), where I work with [Yeyun Gong](https://www.microsoft.com/en-us/research/people/yegong/), [Lei Ji](https://www.microsoft.com/en-us/research/people/leiji/), and [Qi Chen](https://www.microsoft.com/en-us/research/people/cheqi/), and was honored with the **Stars of Tomorrow** award at [Microsoft Research Asia](https://www.microsoft.com/en-us/research/lab/microsoft-research-asia/).

My research interests lie in making large language models more *efficient* and *practical*:
- **Efficient** training and inference methods for LLMs, including cost-efficient inference ([NAACL 2025](https://arxiv.org/abs/2411.15927)), distillation ([ICML 2025](https://arxiv.org/abs/2503.19123), [NAACL 2025](https://arxiv.org/abs/2411.15927)), and data mixture optimization ([ACL 2026F](https://arxiv.org/abs/2508.12116))
- **Real-world impact**, advancing agent adaptability ([NAACL 2025](https://arxiv.org/abs/2411.15927)), scientific discovery ([GenBio 2025](https://arxiv.org/abs/2409.19788), [BioNLP 2025](https://aclanthology.org/2025.bionlp-1.21)), and real-time information access ([NAACL 2024](https://arxiv.org/abs/2311.08329)).


# Work Experience
<div class="work-list">
  {% for w in site.data.work %}
    {% include work-item.html
       logo=w.logo company=w.company role=w.role tenure=w.tenure location=w.location %}
  {% endfor %}
</div>


# Publications
<div class="pub-container">
  <!-- 라디오 버튼 (화면에서 숨김) -->
  <input type="radio" id="tab-selected" name="pub-tabs" checked>
  <input type="radio" id="tab-all" name="pub-tabs">

  <!-- 탭 레이블 (버튼 역할) -->
  <div class="pub-tabs">
    <label for="tab-selected" class="tab-btn btn-sel">Selected</label>
    <label for="tab-all" class="tab-btn btn-all">All Publications</label>
  </div>

  <!-- Selected 리스트 -->
  <div class="pub-list-wrapper selected-list">
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
  </div>

  <!-- All 리스트 -->
  <div class="pub-list-wrapper all-list">
    <div class="pub-list">
      {% for p in site.data.all_publications %}
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
  </div>
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