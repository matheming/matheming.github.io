---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
last_updated: 2026-10-29
excerpt: "Education, experience, publications, and teaching in one place."
redirect_from:
  - /resume
---

{% include base_path %}

<p class="archive__item-meta">Last updated: <time datetime="{{ page.last_updated | date: '%Y-%m-%d' }}">{{ page.last_updated | date: '%B %d, %Y' }}</time></p>

<section class="cv-section">
  <h2 class="archive__section-title">Education</h2>
  <div class="cv-entry">
    <h3>Ph.D. in Statistics</h3>
    <p>University of Science and Technology of China, Since 2025</p>
  </div>
  <div class="cv-entry">
    <h3>M.S. in Applied Statistics</h3>
    <p>University of Science and Technology of China, 2024</p>
  </div>
  <div class="cv-entry">
    <h3>B.S. in Mathematics and Applied Mathematics</h3>
    <p>University of Science and Technology of China, 2021</p>
  </div>
</section>

<section class="cv-section">
  <h2 class="archive__section-title">Work Experience</h2>
  <div class="cv-entry">
    <h3>Teaching Assistant</h3>
    <p>Probability and Mathematical Statistics · 2022.09-2023.02</p>
    <ul class="cv-list">
      <li>Duties included homework correcting and exercise lectures.</li>
      <li>Instructor: Professor Zhishui Hu.</li>
    </ul>
  </div>
  <div class="cv-entry">
    <h3>Internship</h3>
    <p>Supply Chain Y, JD.com · 2022.11-2023.03</p>
    <ul class="cv-list">
      <li>Duties included supply chain causal analysis.</li>
    </ul>
  </div>
</section>

<section class="cv-section">
  <h2 class="archive__section-title">Research</h2>
  <h3>Working Papers</h3>
  <div class="cv-collection">
    {% assign working_papers = site.publications | where: "category", "working_papers" | sort: "date" | reverse %}
    {% for post in working_papers %}
      {% include research-item.html %}
    {% endfor %}
  </div>
  <h3>Publications</h3>
  <div class="cv-collection">
    {% for post in site.publications reversed %}
      {% unless post.category == "working_papers" %}
        {% include research-item.html %}
      {% endunless %}
    {% endfor %}
  </div>
</section>

<section class="cv-section">
  <h2 class="archive__section-title">Talks</h2>
  <div class="cv-collection">
    {% for post in site.talks reversed %}
      <div class="cv-entry">
        <h3><a href="{{ post.paperurl }}">{{ post.title }}</a></h3>
        <p>{{ post.display_date }} &middot; {{ post.location }}</p>
      </div>
    {% endfor %}
  </div>
</section>

<section class="cv-section">
  <h2 class="archive__section-title">Teaching</h2>
  <div class="cv-collection">
    {% for post in site.teaching reversed %}
      {% include archive-single-cv.html %}
    {% endfor %}
  </div>
</section>
