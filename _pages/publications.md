---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  You can also find my work on <u><a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

<h2 id="preprints">Preprints</h2>
{% for post in site.publications reversed  %}
  {% if post.type == "preprint" %}

  {% include archive-single.html %}

  {% endif %}
{% endfor %}
