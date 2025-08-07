---
title: "Sports Analytics Group @ NUS - Team"
layout: gridlay
excerpt: "Sports Analytics Group @ NUS: Team members"
sitemap: false
permalink: /team/
---

# Group Members

## Staff
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
  <p><i>{{ member.institution }}</i></p>
  {% if member.webpage %}
  <p><a href="{{ member.webpage }}" target="_blank" class="btn btn-primary btn-sm">Personal Website</a></p>
  {% endif %}
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


## Master and Bachelor Students


## Current BSc/ MSc students




