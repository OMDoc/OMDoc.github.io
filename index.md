---
layout: default
title: OMDoc Home
---

# OMDoc: Open Mathematical Documents

{% include intro.md %}

[Read more...](about)

## News

{% for post in site.posts %}
{{ post.date | date_to_string }}
: [{{ post.title }}]({{ site.baseurl}}{{ post.url }})
{% endfor %}

<p>&copy; {{ site.time | date: '%Y' }}. All rights reserved.</p>




