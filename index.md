---
layout: home
title: "Cloud Cafes"
subtitle: "Technical documentation and blog"
---

## Recent Posts

{% for post in site.posts limit:10 %}
### [{{ post.title }}]({{ post.url }})
{{ post.date | date: "%B %d, %Y" }} • {{ post.content | strip_html | truncatewords: 30 }}

---
{% endfor %}