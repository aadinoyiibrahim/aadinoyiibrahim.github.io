---
permalink: /
title: "Hi there!"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I completed my PhD in Computer Science with the Physics for Inference and Optimization group led by Prof. Caterina De Bacco at the Max Planck Institute for Intelligent Systems. My work spans interdisciplinary projects—from machine‑learning–driven time‑series prediction and community detection in complex networks to flow optimization in multimodal transport systems. My research interests lie at the intersection of data‑driven modeling, dynamical and nonlinear systems, optimization algorithms, and machine learning.

Outside of my own research, I serve as an Associate Editor for the Journal of Open Research Software (JORS) and peer‑reviewer for several applied‑science journals. I mentor early‑career scientists through Python and data‑science workshops (including TReND in Africa) and co‑organize scientific workshops. I also contribute to open‑source scientific software.

<!-- -------------- two‑column section -------------- -->
<div style="display:flex; flex-wrap:wrap; gap:2rem; margin-top:2rem;">

  <!-- ░░ Column 1 — latest 3 news posts ░░ -->
  <div style="flex:1 1 280px;">
    <h3>News</h3>
    <ul style="margin-left:0; padding-left:0; list-style:none;">
      {% assign news = site.posts
         | where_exp: "p", "p.categories contains 'news'"
         | sort: "date"
         | reverse
         | slice: 0, 3 %}
      {% for post in news %}
        <li style="margin-bottom:0.75rem;">
          <a href="{{ post.url | relative_url }}" style="font-weight:500;">
            {{ post.title }}
          </a><br>
          <small>{{ post.date | date: "%B %d, %Y" }}</small>
        </li>
      {% endfor %}
    </ul>
    <a class="btn btn--primary" href="/news/">More news →</a>
  </div>

  <!-- ░░ Column 2 — education summary ░░ -->
  <div style="flex:1 1 280px;">
    <h3>Education</h3>
    <ul style="margin-left:0;">
      <li><strong>Ph.D. Computer Science</strong><br>
          Max Planck Institute &amp; Univ. Tübingen, 2024
      </li>
      <li><strong>M.Sc. Math &amp; Data Science</strong><br>
          AIMS Senegal, 2019
      </li>
      <li><strong>B.Sc. Mathematics</strong><br>
          Ekiti State University, 2015
      </li>
    </ul>
  </div>

</div>
<!-- ------------ end two‑column section ------------ -->
