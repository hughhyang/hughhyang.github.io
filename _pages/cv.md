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
* [Degree], [Institution], [Year]
* [Degree], [Institution], [Year]
* [Degree], [Institution], [Year]

Work experience
======
* [Start - End]: [Role]
  * [Institution]
  * [Brief responsibility / project]
  * [Supervisor, optional]

* [Start - End]: [Role]
  * [Institution]
  * [Brief responsibility / project]
  * [Supervisor, optional]
  
Skills
======
* [Skill area 1]
* [Skill area 2]
* [Skill area 3]

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* [Service / Leadership 1]
* [Service / Leadership 2]
