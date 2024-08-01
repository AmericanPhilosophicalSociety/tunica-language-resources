---
layout: default
title: "Photographs"
---

# {{ page.title }}

Placeholder explanatory text - <a href="https://diglib.amphilsoc.org/solr-search/content?search_api_fulltext=tunica&sort_by=search_api_relevance&sort_order=DESC&items_per_page=10&f%5B0%5D=genre%3APhotographic%20prints" target="_blank">Mary Haas images</a>

{% assign photos = site.data.photographs | where: "collection", "Mary R. Haas Papers" %}
{% assign dataBsTarget = "HaasCarousel" %}

{% include image-gallery.html %}

Placeholder explanatory text - <a href="https://diglib.amphilsoc.org/solr-search/content?search_api_fulltext=tunica&sort_by=search_api_relevance&sort_order=DESC&items_per_page=10&f%5B0%5D=genre%3APhotographs" target="_blank">Frank G. Speck images</a>

{% assign photos = site.data.photographs | where: "collection", "Frank G. Speck Papers" %}
{% assign dataBsTarget = "SpeckCarousel" %}

{% include image-gallery.html %}

[Also include a listing of all the identified people in the photos, with each name being a link that will show all of the photos in which they are pictured]