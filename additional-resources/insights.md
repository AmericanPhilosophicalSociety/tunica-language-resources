---
layout: default
title: "Insights on the Tunica Language"
permalink: /additional-resources/insights/
---

<h1>{{ page.title }}</h1>
<h2>By Patricia Anderson</h2>

<div class="insights-text">

<p>These short articles were written by Dr. Patricia Anderson, the lead linguist on the NSF project, long time member of the Tunica Language Working Group (or Kuhpani Yoyani Luhchi Yoroni – KYLY) and author of <a href="https://uapress.arizona.edu/book/revitalization-lexicography" target="_blank"><i>Revitalization Lexicography: The Making of the New Tunica Dictionary</i></a> (University of Arizona Press, 2020).</p>

<p>Each article focuses on a particular characteristic of the Tunica language with examples drawn from the <a href="{{ '/notebooks'| relative_url }}">Haas-Youchigant notebooks</a>.</p>

<hr>

</div>

{% assign entries = site.pages | where:"layout", "insights" | sort: "num" %}

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