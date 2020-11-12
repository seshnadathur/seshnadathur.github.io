{% include base_path %}

{% if post.id %}
  {% assign title = post.title | markdownify | remove: "<p>" | remove: "</p>" %}
{% else %}
    {% assign title = post.title %}
{% endif %}

{% if post.arxiv and post.published %}
  [{{post.number}}] **{{post.title}}**, {{post.author}}, {{post.journal}}, ArXiv: [{{post.arxiv_id}}]({{post.arxiv_link}}), [DOI](https://doi.org/{{post.doi}})
{% elsif post.arxiv %}
  [{{post.number}}] **{{post.title}}**, {{post.author}}, {{post.journal}}, ArXiv: [{{post.arxiv_id}}]({{post.arxiv_link}})
{% elsif post.published%}
  [{{post.number}}] **{{post.title}}**, {{post.author}}, {{post.journal}}, [DOI](https://doi.org/{{post.doi}})
{% endif %}
