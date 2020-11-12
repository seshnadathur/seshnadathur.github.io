---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

A list of my publications appears below. An up-to-date version of this list, with added bibliographic and citation information, can be found on the [NASA ADS](https://ui.adsabs.harvard.edu/search/q=%20author%3A%22nadathur%2C%20seshadri%22&sort=date%20desc%2C%20bibcode%20desc&p_=0) system, and a slightly different version is available from the [arXiv](https://arxiv.org/a/nadathur_s_1.html).

### Papers
----
{% include base_path %}

{% for post in site.publications reversed %}
  {% include paper-single.md %}
{% endfor %}

### Conference proceedings
----
{% include base_path %}

{% for post in site.proceedings reversed %}
  {% include proceedings-single.md %}
{% endfor %}
