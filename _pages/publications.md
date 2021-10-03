---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

You can also find my articles on <u><a href="https://scholar.google.com/citations?hl=en&user=YBZt0-AAAAAJ&view_op=list_works&authuser=3">my Google Scholar profile</a>.</u>


{% include base_path %}

{% for post in site.publications reversed %}
    {% if post.venue != '' %}
      {% include archive-single.html %}
    {% endif %}
{% endfor %}


{% unless page.header.overlay_color or page.header.overlay_image %}
  <h1 class="page__title">PREPRINTS</h1>
{% endunless %}

{% for post in site.publications reversed %}
    {% if post.venue == '' %}
      {% include archive-single.html %}
    {% endif %}
{% endfor %}

