---
layout: default
title: 'The Tunica Language Notebooks, Arranged by Topic'
---
# {{ page.title }}

Insert text explaining what these notebooks are and how to access them

{% include view-notebooks.html %}

Text explaining the two different finding aids - TOC and subject matter headings

Maybe some image boxes with links to those?

<button id="expandCollapseButton">Expand/Collapse All</button>

<div class="accordion" id="toc-accordion">
        <div class="accordion-item">
            {% for entry in site.data.notebooks-by-topic %}
                {% assign panelId = "panel" | append: forloop.index %}
                {% assign buttonId = "button" | append: forloop.index %}
                {% assign panelCollapseId = "panelCollapse" | append: forloop.index %}
                {% assign dataBsTarget = "#panelCollapse" | append: forloop.index %}
                <h2 class="accordion-header" id="{{ panelId }}">
                <button class="accordion-button collapsed" type="button" id="{{ buttonId }}" data-bs-toggle="collapse" data-bs-target="{{ dataBsTarget }}" aria-expanded="false" aria-controls="{{ panelCollapseId }}">
                    <h2>
                       {{ entry.topic }}
                    </h2>
                </button>
                </h2>
                <div id="{{ panelCollapseId }}" class="accordion-collapse collapse" aria-labelledby="{{ panelId }}">
                <div class="accordion-body">
                    <ul>
                        {% for section in entry.contents %}
                            <li>
                                {{ section }}
                            </li>
                        {% endfor %}
                    </ul>
                </div>
                </div>
            {% endfor %}
        </div>
</div>