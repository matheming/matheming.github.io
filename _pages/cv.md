---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* M.S. in Applied Statistics, University of Science and Technology of China, 2024
* B.S. in Mathematics and Applied Mathematics, University of Science and Technology of China, 2021

Work experience
======
* 2022.09-2023.02: Teaching Assistant
  * Probability and Mathematical Statistics
  * Duties included: Homework Correcting & Exercise Lecture
  * Teacher: Professor Zhishui Hu
* 2022.11-2023.03: Internship
  * Supply Chain Y, JD.com
  * Duties included: Supply Chain Causal Analysis

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
