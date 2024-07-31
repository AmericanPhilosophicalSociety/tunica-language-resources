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

<div>
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
    {% endfor %}
</div>
