---
permalink: /publications/
title: "Publications"
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">Google Scholar</a>.</div>
{% endif %}

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