---
layout: archive
permalink: /projects/
title: "Math projects and notes."
excerpt: "Some math I've thought about."
author_profile: true
---

I am broadly interested in thinking about **geometrically-flavored problems in algebra**. At the moment, I am most interested in **algebraic topology/homotopy theory**, and have been lucky enough to have some opportunities to explore the field outside of class.

---

{% include base_path %}

{% for post in site.projects reversed %}
  {% include archive-single.html %}
{% endfor %}
