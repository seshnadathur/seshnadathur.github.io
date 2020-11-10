---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

You can find a full list of my publications at [NASA ADS](https://ui.adsabs.harvard.edu/search/q=%20author%3A%22nadathur%2C%20seshadri%22&sort=date%20desc%2C%20bibcode%20desc&p_=0), at [iNSPIRE](https://inspirehep.net/authors/1062279?ui-citation-summary=true), or directly on the [arXiv](https://arxiv.org/a/nadathur_s_1.html).

{% include base_path %}

<!-- {% assign num = site.publications.size %}
{% assign rev_pubs = site.publications reversed %}

{% for i in (1..num) reversed %}
  {{ i }}
{% endfor %} -->

{% for post in site.publications reversed %}
  {% include paper-single.html %}
{% endfor %}
