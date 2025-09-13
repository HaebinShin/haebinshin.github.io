---
permalink: /patents/
title: "Patents"
author_profile: true
---

<h2></h2>

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