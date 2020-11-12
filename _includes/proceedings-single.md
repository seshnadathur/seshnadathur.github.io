{% include base_path %}

{% if post.id %}
  {% assign title = post.title | markdownify | remove: "<p>" | remove: "</p>" %}
{% else %}
    {% assign title = post.title %}
{% endif %}

{% capture line %}
[{{post.number}}] **{{post.title}}**, {{post.author}}, {{post.journal}}
{% endcapture %}
