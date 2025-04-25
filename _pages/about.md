---
permalink: /
title: "Hi there!"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I completed my CS PhD with the *Physics for Inference and Optimization group*, led by <a href="https://www.cdebacco.com">Caterina De Bacco</a>  at the Max Planck Institute for Intelligent Systems. I was a visiting researcher at the GFZ Helmholtz Centre Potsdam.

<!-- My research bridges multiple disciplines—ranging from machine-learning–driven time-series forecasting and community detection in complex networks to optimal-transport models for multimodal traffic flow. I am in data-driven modeling of dynamical and nonlinear systems, developing efficient optimization algorithms and scalable machine-learning frameworks that translate theoretical insights into real-world applications. -->

I am currently an Associate Editor for the <a href="https://openresearchsoftware.metajnl.com/about/editorialteam">Journal of Open Research Software</a> and reviewer for some scientific journals. I am also an active open-source contributor and publishing reproducible code.

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
         | slice: 0, 4 %}
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
          MPI Intelligent Systems &amp; Uni-Tübingen, 2024
      </li>
      <li><strong>M.Sc. Math &amp; Data Science</strong><br>
          AIMS-Senegal, 2019
      </li>
      <li><strong>B.Sc. Mathematics</strong><br>
          Ekiti State University, 2015
      </li>
    </ul>
  </div>

</div>
<!-- ------------ end two‑column section ------------ -->
