---
layout: archive
title: "Publications (# indicates the corresponding author)"
permalink: /publications/
author_profile: false
---

<br>

<!--<hr style="border:none; height:2px; background-color:rgb(245,245,245); margin:20px auto;">-->

# <span style="font-family:Times New Roman;text-decoration:underline;color:rgb(25,25,112);">Journal & Magazine Papers</span>
## 2025
  1. **Y. Wei**, Q. Ye, W. Zhuang and X. Shen, "Energy-efficient multi-user adaptive 360° video streaming: A two-step approach with device video super-resolution," *IEEE Transactions on Network Science and Engineering*, early access, Oct. 3, 2025, doi: 10.1109/TNSE.2025.3617381.
  2. **Y. Wei**, Q. Ye, K. Qu, W. Zhuang and X. Shen, "E2E performance modeling for slice-based video streaming with layered encoding," *IEEE Transactions on Networking*, early access, Jul. 31, 2025, doi: 10.1109/TON.2025.3591401.
  3. **Y. Wei**, Q. Ye, K. Qu, W. Zhuang and X. Shen, "Customized transmission protocol for tile-based 360° VR video streaming over core network slices," *IEEE/ACM Transactions on Networking*, vol. 33, no. 1, pp. 340-354, 2025.

## 2020 and before
  1. 唐伦, **魏延南#**, 谭颀, 唐睿, 陈前斌. H-CRAN网络下联合拥塞控制和资源分配的网络切片动态资源调度策略[J]. 电子与信息学报, 2020, 42(5): 1244-1252. doi: 10.11999/JEIT190439
  2. 唐伦, **魏延南#**, 马润琳, 贺小雨, 陈前斌. 虚拟化云无线接入网络下基于在线学习的网络切片虚拟资源分配算法[J]. 电子与信息学报, 2019, 41(7): 1533-1539. doi: 10.11999/JEIT180771
  3. L. Tang, **Y. Wei#**, et al., "Queue-aware dynamic resource reuse and joint allocation algorithm in self-backhaul small cell networks," *IEEE Access*, vol. 6, pp. 61077-61090, 2018.
  4. L. Tang, **Y. Wei#**, et al., "Delay-aware dynamic resource allocation and ABS configuration algorithm in HetNets based on Lyapunov optimization," *IEEE Access*, vol. 5, pp. 23764-23775, 2017.

<br>

<!--<hr style="border:none; height:2px; background-color:rgb(245,245,245); margin:20px auto;">-->

# <span style="font-family:Times New Roman;text-decoration:underline;color:rgb(25,25,112);">Conference Papers</span>
## 2025
  1. **Y. Wei**, Q. Ye, W. Zhuang and X. Shen, "Energy-efficient multi-user adaptive 360° video streaming with device video super-resolution", in *Proc. IEEE Globecom Workshops (GC Wkshps)*, Taipei, Taiwan, to appear.

## 2024
  1. **Y. Wei**, Q. Ye, K. Qu, W. Zhuang and X. S. Shen, "Transmission protocol customization for on-demand tile-based 360° VR video streaming," in *Proc. IEEE/CIC International Conference on Communications in China (ICCC)*, Hangzhou, China, July 2024. <span style="color:rgb(227,23,13);">(Best Paper Award)</span>

<br>

<!--<hr style="border:none; height:2px; background-color:rgb(245,245,245); margin:20px auto;">-->

# <span style="font-family:Times New Roman;text-decoration:underline;color:rgb(25,25,112);">Patents</span>
  1. 陈前斌, 马润琳, **魏延南**, 等. 一种在F-RAN架构中联合资源分配和内容缓存的方法. 发明专利 (已授权), CN109951849B, 中国, 2023.
  2. 陈前斌, 管令进, **魏延南**, 等. 一种基于深度强化学习的异构云无线接入网资源分配方法. 发明专利 (已授权), CN110493826B, 中国, 2022.
  3. 陈前斌, **魏延南**, 等. H-CRAN网络下联合拥塞控制和资源分配的网络切片动态资源调度方法. 发明专利 (已授权), CN110809261B, 中国, 2022.
  4. 唐伦, 肖娇, **魏延南**, 等. 一种基于能效的NOMA蜂窝车联网动态资源调度方法. 发明专利 (已授权), CN109905918B, 中国, 2022.
  5. 陈前斌, **魏延南**, 等.一种带内全双工系统无线接入与回传联合资源分配方法. 发明专利 (已授权), CN108964806B, 中国, 2021.














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
