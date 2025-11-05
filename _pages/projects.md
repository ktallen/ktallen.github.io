---
layout: archive
permalink: /research/
title: "Research"
excerpt: "Some math I've thought about."
author_profile: true
---

Here is some extra information on projects I have been involved in. Click the link for more details on the project. If you have any questions, please don't hesitate to reach out!

{% include base_path %}
{% for post in site.projects reversed %}
  {% include archive-single.html %}
{% endfor %}

---
## Undergraduate projects

These are some rough drafts from undergraduate research work. There are some known mistakes and possibly more unknown ones, but I'll leave them here for now in case they can be of use. 
{% include base_path %}
{% for post in site.undergradprojects reversed %}
  {% include archive-single.html %}
{% endfor %}
