---
layout: photos
display-title: 'Photographs by Subject'
title: 'Photographs by Subject'
---

[Placeholder explanatory text]

## Pictured

{% assign pictured = site.data.photo-subjects | sort: 'name' %}

<div>
    {% for person in pictured %}
        {% unless person.photographed == "n" %}
            <p>
                <a href="https://diglib.amphilsoc.org/taxonomy/term/{{ person.taxonomy }}" target="_blank" class="no-decoration-link">
                    {{ person.name }}
                </a>
            </p>
        {% endunless %}
    {% endfor %}
</div>

{% assign creators = site.data.photo-subjects | where:"photographer", "y" | sort: 'name' %}

## Creator/Photographer

<div>
    {% for person in creators %}
        <p>
            <a href="https://diglib.amphilsoc.org/taxonomy/term/{{ person.taxonomy }}" target="_blank" class="no-decoration-link">
                {{ person.name }}
            </a>
        </p>
    {% endfor %}
</div>