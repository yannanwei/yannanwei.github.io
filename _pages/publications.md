---
layout: archive
title: "Publications (# indicates the corresponding author)"
permalink: /publications/
author_profile: false
---

<br>
# Journal & Magazine Papers
## <span style="color:blue;">2025</span>
  3. Device-VSR-Assisted 360° Streaming with Edge Scheduling, *IEEE GLOBECOM Workshops*, 2025.


# Conference Papers

<br>
# Patents



















{% comment %}
<!-- publications.html -->
{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

<!-- New style rendering if publication categories are defined -->
{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h2>{{ category[1].title }}</h2><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}
{% endcomment %}
