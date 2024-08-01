---
layout: default
title: 'Oral Histories'
---
# {{ page.title }}

<!-- <p class="text-align-center">
    <video controls="" height="315" width="560">
        <source src="https://diglib.amphilsoc.org/_flysystem/fedora/2023-12/340448-Service%20File.mp4" type="video/ogg">
        <source src="https://diglib.amphilsoc.org/_flysystem/fedora/2023-12/340448-Service%20File.mp4" type="video/mp4">
    </video>
</p> -->

<div>
    {% include oral-histories-nav.html %}
</div>

<!-- <div>
    {% assign categories = site.oral-histories | where:"layout", "oral-history-category" %}
    {% for page in categories %}
        <p><a href="{{ page.url | relative_url }}">{{ page.title }}</a></p>
    {% endfor %}
</div> -->

{% assign featured = "Who was Sesostrie Youchigant?, Rabbit Dance Song, Teaching Younger Generations, On Language Reawakening, Continuing traditional Tunica crafts" | split: ", " %}

<div>
    {% for title in featured %}
        {% assign video = site.oral-histories | where:"title", title | first %}
        {% include video-embed-flex.html %}
        <!-- <div class='box-wrapper'>
            <div class='box'>
                {% assign categoryRecord = site.oral-histories | where:"title", video.category | first %}
                <a href="{{  categoryRecord.url | relative_url }}">
                    <p>Learn More About {{ video.category }}</p>
                </a>
            </div>
        </div> -->
        <!-- Alternative look with button - width settings don't work -->
        <!-- <div class="d-grid gap-2">
            <a href="{{  categoryRecord.url | relative_url }}">
                <button class="btn btn-primary" type="button">Learn More About {{ video.category }}</button>
            </a> 
        </div> -->
        {% unless forloop.last %}
            <hr>
        {% endunless %}
    {% endfor %}
</div>

<!-- <div>
    {% assign videos = site.oral-histories | where:"layout", "video" %}
    {% for video in videos %}
        <div>
            <h3>{{ video.title }}</h3>
            <video controls="" height="315" width="560">
                <source src="{{ video.link }}" type="video/ogg">
                <source src="{{ video.link }}" type="video/mp4">
            </video>
            {% if video.interviewee %}
                <p>Interviewee: {{ video.interviewee }}</p>
            {% endif %}
            <p><a href="{{ video.url | relative_url }}">Video page</a></p>
        </div>
        {% include video-embed.html %}
    {% endfor %}
</div> -->
