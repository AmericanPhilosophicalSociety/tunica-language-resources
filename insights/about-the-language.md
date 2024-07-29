---
layout: insights
title: "Insights on the Tunica Language"
---

A few introductory sentences/paragraphs about these posts, the author, etc.?

<!-- <ul>
  {% for page in site.pages %}
    {% if page.layout == 'insights' and page.title != "Introduction: Insights on the Tunica Language" %}
        <li>
            <a href="{{ page.url | relative_url }}">{{ page.title }}</a>
            <p>{{ page.excerpt }}</p>
            <a href="{{ page.url | relative_url }}">Read more</a>
        </li>
    {% endif %}
  {% endfor %}
</ul> -->

{% tablerow page in site.pages %}
    {% if page.layout == 'insights' and page.title != "Introduction: Insights on the Tunica Language" %}
        <div class="card gap-3 mx-3" style="width: 60rem;" padding="$spacer !important;">
            <div class="card-body" padding="$spacer !important;">
                        <h5 class="card-title"><a href="{{ page.url | relative_url }}">{{ page.title }}</a></h5>
                        <h6 class="card-subtitle mb-2 text-body-secondary">By {{ page.author }}</h6>
                        <p class="card-text">{{ page.excerpt }}</p>
                        <a href="{{ page.url | relative_url }}">Read more</a>
            </div>  
        </div>
    {% endif %}
{% endtablerow %}