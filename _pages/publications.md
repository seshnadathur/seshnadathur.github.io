---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<html>
<head>
<script type="text/javascript">
<!--
var arxiv_authorid="nadathur_s_1";
var arxiv_format="arxiv";
var arxiv_max_entries=0;         // show all articles
var arxiv_includeSummary=1;      // show abstracts
var arxiv_includeComments=0;     // do not show comments
var arxiv_includeSubjects=0;     // do not show subjects
var arxiv_includeJournalRef=0;   // do not show journal reference (but do show DOI)
//--></script>
<style type="text/css">
// styles must be entered here to override default arXiv styles embedded by js
div#arxivfeed div#arxivcontainer div.meta p {font-style: italic;}
div#arxivfeed div#arxivcontainer div.meta div.list-authors {
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  max-width: 700px;
}
</style>
<script type="text/javascript" src="https://arxiv.org/js/myarticles.js">
</script>
</head>

<body>
<p>Feed should appear here?</p>
<div id="arxivfeed"></div>
</body>
</html>

You can find a full list of my publications at [NASA ADS](https://ui.adsabs.harvard.edu/search/q=%20author%3A%22nadathur%2C%20seshadri%22&sort=date%20desc%2C%20bibcode%20desc&p_=0), at [iNSPIRE](https://inspirehep.net/authors/1062279?ui-citation-summary=true), or directly on the [arXiv](https://arxiv.org/a/nadathur_s_1.html).

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
