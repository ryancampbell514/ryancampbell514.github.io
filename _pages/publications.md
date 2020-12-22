---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

#{% for post in site.publications reversed %}
#  {% include archive-single.html %}
#{% endfor %}

<h2 id="preprints">Preprints</h2>
{% for post in site.publications reversed  %}
  {% if post.type == "preprint" %}


  <ul>
  {% include archive-single.html %}  #{% include publication-item.html %}
  </ul>

  {% endif %}
{% endfor %}
