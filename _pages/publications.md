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
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="40%" style="float: left" />
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

<!-- Group by year and sort in descending order -->
{% assign sorted_publist = site.data.publist | group_by_exp: "pub", "pub.year" | sort: "name" | reverse %}

{% for year_group in sorted_publist %}
  <h3 class="year">{{ year_group.name }}</h3>
  <ol class="bibliography">
    {% for publi in year_group.items %}
      <li>
        <div class="row">
          <div class="col-sm-12" display="block">
            <b>{{ publi.title }}</b><br />
            <em>{{ publi.authors }}</em><br />
            <i>{{ publi.link.display }}</i>, {{ publi.year }}
            
            <br />

            {% if publi.link.url %}
              <a href="{{ publi.link.url }}" target="_blank"><button class="btn-arxiv">Paper</button></a> 
            {% endif %}

            {% if publi.link.code %}
              <a href="{{ publi.link.code }}" target="_blank"><button class="btn-code">Code</button></a> 
            {% endif %}

            {% if publi.abstract %}
              <a data-toggle="collapse" href="#{{ publi.id }}-abstract" class="btn-abstract" role="button">ABS</a>
            {% endif %}

            {% if publi.bibtex %}
              <a data-toggle="collapse" href="#{{ publi.id }}-bib" class="btn-bib" role="button">BIB</a>
            {% endif %}

            {% if publi.abstract %}
            <div class="collapse" id="{{ publi.id }}-abstract">
              <div class="well-abstract">
                {{ publi.abstract }}
              </div>
            </div>
            {% endif %}

            {% if publi.bibtex %}
            <div class="collapse" id="{{ publi.id }}-bib">
              <div class="well-bib">
                <pre><code class="language-bibtex">{{ publi.bibtex }}</code></pre>
              </div>
            </div>
            {% endif %}
          </div>
        </div>
      </li>
    {% endfor %}
  </ol>
{% endfor %}
