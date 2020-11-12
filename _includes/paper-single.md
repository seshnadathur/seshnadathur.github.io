{% include base_path %}

{% if post.id %}
  {% assign title = post.title | markdownify | remove: "<p>" | remove: "</p>" %}
{% else %}
  {% assign title = post.title %}
{% endif %}

{% if post.reviewed %}
  [{{post.number}}]. **{{post.title}}**, {{post.author}}, [{{post.journal}}](https://doi.org/{{ post.doi }}), ArXiv: [{{post.arxiv_id}}]({{post.arxiv_link}})
{% else %}
  [{{post.number}}]. **{{post.title}}**, {{post.author}}, ArXiv: [{{post.arxiv_id}}]({{post.arxiv_link}})
{% endif %}
