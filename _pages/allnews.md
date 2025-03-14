---
title: "News"
layout: textlay
excerpt: "Sports Analytics Group @ NUS"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }}<br><p>{{ article.headline | markdownify}}</p>
<br></p>
{% endfor %}
