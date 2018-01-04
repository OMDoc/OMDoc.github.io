---
layout: default
title: OMDoc Home
---

# OMDoc: Open Mathematical Documents

{% include intro.md %}

[Read more...](about)

## News ([all/older news](news/))

{% for post in site.posts %}
{% if forloop.index < 8 %}
*  {{ post.date | date_to_string }} : [{{ post.title }}]({{ site.baseurl}}{{ post.url }})
{% endif %}
{% endfor %}

<p>&copy; {{ site.time | date: '%Y' }}. All rights reserved.</p>




