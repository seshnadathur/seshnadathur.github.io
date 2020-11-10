---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<script type="text/javascript">
<!--
var arxiv_authorid = "nadathur_s_1";
//--></script>
<script type="text/javascript" src="https://arxiv.org/js/myarticles.js"></script>

You can find a full list of my publications at [NASA ADS](https://ui.adsabs.harvard.edu/search/q=%20author%3A%22nadathur%2C%20seshadri%22&sort=date%20desc%2C%20bibcode%20desc&p_=0), at [iNSPIRE](https://inspirehep.net/authors/1062279?ui-citation-summary=true), or directly on the [arXiv](https://arxiv.org/search/astro-ph?searchtype=author&query=Nadathur%2C+S).

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

<div id="arxivfeed"></div>
