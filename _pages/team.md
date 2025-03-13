---
title: "Sports Analytics Group @ NUS - Team"
layout: gridlay
excerpt: "Sports Analytics Group @ NUS: Team members"
sitemap: false
permalink: /team/
---

# Group Members
 
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left; margin-right: 15px;" />
  <h4>{{ member.name }}</h4>
  <p><i>{{ member.info }}</i></p>
  <p><i>{{ member.institution }}</i></p>

  {% if member.website %}
  <p><a href="{{ member.website }}" target="_blank" class="btn btn-primary btn-sm">Personal Website</a></p>
  {% endif %}
</div>

{% assign number_printed = number_printed | plus: 1 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% if number_printed | modulo: 2 == 1 %}
</div>
{% endif %}
