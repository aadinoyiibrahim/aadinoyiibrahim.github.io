---
permalink: /
title: "Hi there!"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---



I'm a Data Scientist and Software Engineer with a PhD in Computer Science. Currently, I work as **Postdoc (Data Scientist)** at <a href="https://synosys.github.io/authors/abdullahi/">TU Dresden</a>. Previously, I completed my CS PhD with the *Physics for Inference and Optimization group*, led by <a href="https://www.cdebacco.com">Caterina De Bacco</a>  at the Max Planck Institute for Intelligent Systems, and was a visiting researcher at GFZ Helmholtz Centre Potsdam. I am currently an Associate Editor for the <a href="https://openresearchsoftware.metajnl.com/about/editorialteam">Journal of Open Research Software</a> and reviewer for some scientific journals. I am also an active open-source contributor.

<!-- ### Hi there!
My research bridges multiple disciplines—ranging from machine-learning–driven time-series forecasting and community detection in complex networks to optimal-transport models for multimodal traffic flow. I am in data-driven modeling of dynamical and nonlinear systems, developing efficient optimization algorithms and scalable machine-learning frameworks that translate theoretical insights into real-world applications. -->


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
    <h3>Latest blogs</h3>
    <ul style="margin-left:0;">
      <li><strong><a href="https://medium.com/best-open-source-linear-programming-solver/best-open-source-linear-programming-solver-2395c1f9070e">Best Open‑Source Linear Programming Solver</a></strong><br>
      </li>
      <li><strong><a href="https://medium.com/capacitated-facility-location-mip-with-open-source/capacitated-facility-location-mip-with-open-source-solvers-201d1eb88b79">Capacitated Facility-Location MIP with Open-Source Solvers</a></strong><br>
      </li>
      <li><strong><a href="https://www.baeldung.com/cs/best-open-source-mixed-integer-optimization-solver">Best Open-Source Mixed Integer Optimization Solver
</a></strong><br>
      </li>
    </ul>
  </div>

</div>
<!-- ------------ end two‑column section ------------ -->
