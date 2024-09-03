---
layout: default
title: "Insights on the Tunica Language"
---

<h1>{{ page.title }}</h1>
<h2>By Patricia Anderson</h2>

[Placeholder text: A few introductory sentences/paragraphs about these posts, the author, etc.?]

{% assign entries = site.pages | where:"layout", "insights" %}

<div>
    {% for page in entries %}
        <div class="insights-text">
            <h2><a href="{{ page.url | relative_url }}">{{ page.title }}</a></h2>
            <!-- <h3>By {{ page.author }}</h3> -->
            <p>{{ page.excerpt }}</p>
            <p class="read-more"><a href="{{ page.url | relative_url }}">Read more</a></p>
            {% unless forloop.last == true %}
                <hr>
            {% endunless %}
        </div>
    {% endfor %}
</div>