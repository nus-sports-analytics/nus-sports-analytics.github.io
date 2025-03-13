---
title: "Sports Analytics Group @ NUS - Publications"
layout: gridlay
excerpt: "Sports Analytics Group @ NUS -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

## Group Highlights
(At the end of this page, you can find the [full list of publications](#full-list-of-publications).)

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix">
    <div class="well">
      <pubtit>{{ publi.title }}</pubtit>
<!--       <p><img src="/images/pubpic/{{ publi.image }}" class="img-responsive" width="40%" style="float: left" /></p> -->
      <p>{{ publi.description }}</p>
      <p><em>{{ publi.authors }}</em></p>
      <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
      <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
      <p> {{ publi.news2 }}</p>
    </div>
  </div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


## List of Publications

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
