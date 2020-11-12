{% include base_path %}

{% if post.id %}
  {% assign title = post.title | markdownify | remove: "<p>" | remove: "</p>" %}
{% else %}
    {% assign title = post.title %}
{% endif %}

{% capture line %}
[{{post.number}}] **{{post.title}}**, {{post.author}}, {{post.journal}}
{% endcapture %}
{% if post.arxiv %}
  {% capture arxiv_line %}
  {{line}}, ArXiv: [{{post.arxiv_id}}]({{post.arxiv_link}})
  {% endcapture %}
{% else %}
  {% capture arxiv_line %}
  {{line}}
  {% endcapture %}
{% endif %}
{% if post.published %}
  {{arxiv_line}}, [DOI](https://doi.org/{{post.doi}})
{% else %}
  {{arxiv_line}}
{% endif %}
