---
layout: archive
title: "Publications (# indicates the corresponding author)"
permalink: /publications/
author_profile: false
---

<br>

<hr style="border:none; height:2px; background-color:rgb(65,105,255); margin:20px auto;">

# <span style="font-family:Times New Roman;text-decoration:underline;color:rgb(65,105,255);">Journal & Magazine Papers</span>
## 2025
  1. **Y. Wei**, Q. Ye, W. Zhuang and X. Shen, "Energy-efficient multi-user adaptive 360° video streaming: A two-step approach with device video super-resolution," *IEEE Transactions on Network Science and Engineering*, early access, Oct. 3, 2025, doi: 10.1109/TNSE.2025.3617381.
  2. 

<br>

<hr style="border:none; height:2px; background-color:rgb(65,105,255); margin:20px auto;">

# <span style="font-family:Times New Roman;text-decoration:underline;color:rgb(65,105,255);">Conference Papers</span>

<br>

<hr style="border:none; height:2px; background-color:rgb(65,105,255); margin:20px auto;">

# <span style="font-family:Times New Roman;text-decoration:underline;color:rgb(65,105,255);">Patents</span>
















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
