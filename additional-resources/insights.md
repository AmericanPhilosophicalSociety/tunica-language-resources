---
layout: default
title: "Insights on the Tunica Language"
---

<h1>{{ page.title }}</h1>

[Placeholder text: A few introductory sentences/paragraphs about these posts, the author, etc.?]

{% tablerow page in site.pages %}
    {% if page.layout == 'insights' %}
        <div class="card gap-3 mx-3" style="width: 70rem;" padding="$spacer !important;">
            <div class="card-body" padding="$spacer !important;">
                        <h2 class="card-title"><a href="{{ page.url | relative_url }}">{{ page.title }}</a></h2>
                        <h3 class="card-subtitle mb-2 text-body-secondary">By {{ page.author }}</h3>
                        <p class="card-text">{{ page.excerpt }}</p>
                        <h4><a href="{{ page.url | relative_url }}">Read more</a></h4>
            </div>  
        </div>
    {% endif %}
{% endtablerow %}