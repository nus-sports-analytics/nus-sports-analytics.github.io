---
title: "Sports Analytics Group @ NUS - Team"
layout: gridlay
excerpt: "Sports Analytics Group @ NUS: Team members"
sitemap: false
permalink: /team/
---

# Group Members

Jump to [staff](#staff), [master and bachelor students](#master-and-bachelor-students), [alumni](#alumni), [administrative support](#administrative-support), [lab visitors](#lab-visitors).

## Staff  
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

  <ul style="overflow: hidden;">
    {% for i in (1..5) %}
      {% assign education_key = 'education' | append: i %}
      {% if member[education_key] %}
        <li>{{ member[education_key] }}</li>
      {% endif %}
    {% endfor %}
  </ul>

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

---

## Master and Bachelor Students  
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <h4>{{ member.name }}</h4>
  <p><i>{{ member.info }}</i></p>

  <ul style="overflow: hidden;">
    {% for i in (1..4) %}
      {% assign education_key = 'education' | append: i %}
      {% if member[education_key] %}
        <li>{{ member[education_key] }}</li>
      {% endif %}
    {% endfor %}
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% if number_printed | modulo: 2 == 1 %}
</div>
{% endif %}

---

## Alumni  
{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left; margin-right: 15px;" />
  <h4>{{ member.name }}</h4>
  <p><i>{{ member.duration }} <br> Role: {{ member.info }}</i></p>
</div>

{% assign number_printed = number_printed | plus: 1 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% if number_printed | modulo: 2 == 1 %}
</div>
{% endif %}

---

## Former Visitors, BSc/MSc Students  
<div class="row">
  <div class="col-sm-4">
    <h4>Visitors</h4>
    {% for member in site.data.alumni_visitors %}
    <p>{{ member.name }}</p>
    {% endfor %}
  </div>

  <div class="col-sm-4">
    <h4>Master Students</h4>
    {% for member in site.data.alumni_msc %}
    <p>{{ member.name }}</p>
    {% endfor %}
  </div>

  <div class="col-sm-4">
    <h4>Bachelor Students</h4>
    {% for member in site.data.alumni_bsc %}
    <p>{{ member.name }}</p>
    {% endfor %}
  </div>
</div>


## Administrative Support
<a href="mailto:Rijsewijk@Physics.LeidenUniv.nl">Ellie van Rijsewijk</a> is helping us (and other groups) with administration.
