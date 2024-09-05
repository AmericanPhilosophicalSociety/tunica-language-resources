---
layout: default
title: "Photographs"
---

# {{ page.title }}

<h2><a href="{{ '/additional-resources/photo-subjects' | relative_url }}">See list of photo subjects</a></h2>

Placeholder explanatory text - <a href="https://diglib.amphilsoc.org/solr-search/content?search_api_fulltext=tunica&sort_by=search_api_relevance&sort_order=DESC&items_per_page=10&f%5B0%5D=genre%3APhotographic%20prints" target="_blank">Mary Haas images</a>

Placeholder explanatory text - <a href="https://diglib.amphilsoc.org/solr-search/content?search_api_fulltext=tunica&sort_by=search_api_relevance&sort_order=DESC&items_per_page=10&f%5B0%5D=genre%3APhotographs" target="_blank">Frank G. Speck images</a>

[Also include a listing of all the identified people in the photos, with each name being a link that will show all of the photos in which they are pictured]

{% assign photos = site.data.photographs | where: "collection", "Mary R. Haas Papers" %}
{% assign photo1 = photos | first %}
{% assign photo1ImgPath = "/assets/img/" | append: photo1.fileName %}

<div class="photo-gallery">
<!-- The grid: four columns -->
<div class="row">
{% for photo in photos %}
{% assign imgPath = "/assets/img/" | append: photo.fileName %}
{% assign imgId = "img" | append: forloop.index %}
  <div class="column">
    <img src="{{ imgPath | relative_url }}" alt="Insert alt text" id="{{ imgId }}" onclick="myFunction(this);">
  </div>
{% endfor %}
</div>

{% for photo in photos %}
{% assign imgPath = "/assets/img/" | append: photo.fileName %}
{% assign divId = "img" | append: forloop.index | append: "expanded" %}
<!-- The expanding image container -->

{% if forloop.index == 1 %}
<div class="container" id="{{ divId }}" style="display: block">
{% else %}
<div class="container" id="{{ divId }}" style="display: none">
{% endif %}

  <!-- Expanded image -->
  <img src="{{ imgPath | relative_url }}" style="width:100%">

  <!-- Image text -->
  <div>
    <p>{{ photo.title }}</p>
    <p>{{ photo.description }}</p>
  </div>
</div>
{% endfor %}
</div>

<script>
    function myFunction(img) {
    // query selector (all?): div class container, display style = block
    // change display style to hidden
    let currentContainer = document.querySelector(".container[style*='display: block']");
    currentContainer.style.display = "none";

    let imgId = img.id + "expanded";
    let div = document.getElementById(imgId);
    div.style.display = "block";

    // use image ID to get the correct container div
    // set that one to display = block while the others are hidden
    }
</script>