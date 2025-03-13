---
title: "Sports Analytics Group @ NUS - Home"
layout: homelay
excerpt: "Sports Analytics Group at National University of Singapore"
sitemap: false
permalink: /
---

Welcome to the **Sports Analytics Group @ NUS**, where we integrate cutting-edge computational techniques with sports science to revolutionize performance analysis, strategic decision-making, and athlete development.  

<!-- Add custom CSS inside a <style> block within a Markdown file -->
<style>
    /* Ensure all images in the carousel have the same size */
    .carousel-inner .item img {
        width: 100%; /* Make images responsive */
        height: 500px; /* Set a fixed height for uniformity */
        object-fit: cover; /* Crop images while maintaining aspect ratio */
    }

    /* Ensure the carousel itself has a fixed height */
    .carousel-inner {
        height: 500px;
    }

    /* Center images in case they have different widths */
    .carousel-inner .item {
        text-align: center;
    }
</style>

<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="4000" data-pause="hover">
    <!-- Menu -->
    <ol class="carousel-indicators">
        <li data-target="#carousel" data-slide-to="0" class="active"></li>
        <li data-target="#carousel" data-slide-to="1"></li>
        <li data-target="#carousel" data-slide-to="2"></li>
        <li data-target="#carousel" data-slide-to="3"></li>
        <li data-target="#carousel" data-slide-to="4"></li>
        <li data-target="#carousel" data-slide-to="5"></li>
    </ol>

    <!-- Items -->
    <div class="carousel-inner" markdown="0">
        <div class="item active">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/isace24.JPG" alt="Slide 1">
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/djokovic.jpg" alt="Slide 2">
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/john.jpg" alt="Slide 3">
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/pmc.jpg" alt="Slide 4">
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/pipeline.jpg" alt="Slide 5">
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider7001400/vid2seq.png" alt="Slide 6">
        </div>
    </div>

    <!-- Controls -->
    <a class="left carousel-control" href="#carousel" role="button" data-slide="prev">
        <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
    </a>
    <a class="right carousel-control" href="#carousel" role="button" data-slide="next">
        <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
    </a>
</div>

<!-- Include Bootstrap JS (ensure this is in the template/layout that loads this Markdown file) -->
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>


## About Us
Led by **Professor [Dong Jin Song](https://www.comp.nus.edu.sg/~dongjs/)**, our research focuses on Sports Analytics, a highly interdisciplinary field combining probabilistic reasoning, computer vision, and machine learning to extract deep insights from game dynamics. Our work spans multiple sports, such as tennis, badminton, basketball, and American football, driving innovation in match strategy, player performance optimization, and tactical analysis. Beyond research, we actively collaborate with academic institutions, sports organizations, and industry partners to bridge the gap between theory and real-world applications. We are also the organizers of the International Sports Analytics Conference and Exhibition ([ISACE](https://formal-analysis.com/isace/2025/)), a global platform uniting experts in academia, industry, and professional sports.  

## Depintel - SportsInsight  
Our research has led to the founding of [Depintel](https://depintel.com/index.html), a technology-driven company dedicated to transforming sports through advanced data analytics. Our flagship product, [SportsInsight](https://depintel.pythonanywhere.com/), provides state-of-the-art insight analytics for professional tennis players, offering:  
- Comprehensive match analysis using AI-powered models.  
- Opponent scouting and tactical recommendations for pre-match preparation.  
- Automated video breakdown for fast, fine-grained event detection and strategy formulation.  

SportsInsight is designed to empower players and coaches with deep, data-driven intelligence, enhancing competitive performance at the highest levels.  

## Global Collaboration 
Beyond research and product development, we actively collaborate with academic institutions, sports organizations, and industry partners to bridge the gap between theory and real-world applications. We are also the organizers of the International Sports Analytics Conference and Exhibition (ISACE), a global platform uniting experts in academia, industry, and professional sports.  

At NUS, we are committed to pushing the boundaries of sports intelligence—transforming raw data into actionable insights for the future of competitive sports.  


<figure class="fourth">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_Leiden.jpg" style="width: 210px">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_Nanofront.jpg" style="width: 110px">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_NWO.jpg" style="width: 120px">
  <img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Logo_ERC.jpg" style="width: 110px">
</figure>
