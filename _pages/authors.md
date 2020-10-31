---
layout: page
title: Authors
permalink: /authors/
image: '/images/26.jpg'
published: false
---

{% for author in site.authors %}
## {{ author.name }}
{% if author.avatar %}
<a href="{{ author.url }}" class="article__author-image" aria-label="{{author.avatar}}'s Picture"><img class="lazy" data-src="{{site.baseurl}}{{author.avatar}}" alt="{{author.name}}'s Picture"></a>
{% endif %}
{{ author.content }}
{% endfor %}


