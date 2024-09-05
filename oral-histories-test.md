---
layout: default
---

<h1>Oral Histories</h1>

<div>
    {% include oral-histories-nav.html %}
</div>

{% assign featured = "Who was Sesostrie Youchigant?, Rabbit Dance Song, Teaching Younger Generations, On Language Reawakening, Continuing traditional Tunica crafts" | split: ", " %}

<div>
    {% for title in featured %}
        {% assign video = site.oral-histories | where:"title", title | first %}
        {% include video-embed-alternate.html %}
        {% unless forloop.last %}
            <hr>
        {% endunless %}
    {% endfor %}
</div>