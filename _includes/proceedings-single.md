{% include base_path %}

{% if post.id %}
  {% assign title = post.title | markdownify | remove: "<p>" | remove: "</p>" %}
{% else %}
  {% assign title = post.title %}
{% endif %}

{% capture line %}
[{{post.number}}]. *{{post.title}}*, {{post.author}}, {{post.journal}}
{% endcapture %}
{% if post.arxiv %}
  {% capture line %}
  {{line}}, ArXiv: [{{post.arxiv_id}}]({{post.arxiv_link}})
  {% endcapture %}
{% endif}
{% if post.published %}
  {{line}}, [DOI](https://doi.org/{{ post.doi }})
{% else %}
  {{line}}
{% endif %}
