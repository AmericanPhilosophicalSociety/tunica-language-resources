---
layout: default
title: 'Oral Histories'
---
# {{ page.title }}

Placeholder text

<!-- <p class="text-align-center">
    <video controls="" height="315" width="560">
        <source src="https://diglib.amphilsoc.org/_flysystem/fedora/2023-12/340448-Service%20File.mp4" type="video/ogg">
        <source src="https://diglib.amphilsoc.org/_flysystem/fedora/2023-12/340448-Service%20File.mp4" type="video/mp4">
    </video>
</p> -->

<div>
    {% for video in site.oral-histories %}
        <div>
            <video controls="" height="315" width="560">
                <source src="{{ video.link }}" type="video/ogg">
                <source src="{{ video.link }}" type="video/mp4">
            </video>
            <p><a href="{{ video.url | relative_url }}">Video page</a></p>
        </div>
    {% endfor %}
</div>
