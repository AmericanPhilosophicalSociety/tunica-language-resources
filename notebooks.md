---
layout: default
title: 'The Tunica Language Notebooks'
parallax: true
image:
  img_url: '/womeninscience/assets/img/tunica-notebook-3.jpg'
  img_alt: A blue notebook with a Yale University logo and handwritten text reading "Tunica III".
  caption_url: 'https://diglib.amphilsoc.org/islandora/object/women-science-nd/'
  caption: Mary Haas's Tunica notebooks
---

# {{ page.title }}

Insert text explaining what these notebooks are and how to access them

{% include view-notebooks.html %}

Text explaining the two different finding aids - TOC and subject matter headings

Maybe some image boxes with links to those?

<script>
    $("#collapseAll").click( function() {
        let button = document.getElementById("collapseAll");
        if(!$('.accordion-header').hasClass("active")){
            $('.accordion-header').removeClass("active").addClass("active");
            button.innerHTML = 'Collapse all'

        } else {
            $('.accordion-header').addClass("active").removeClass("active");
            button.innerHTML = 'Expand all'
        }
    });
</script>

<button id="collapseAll">Button Text</button>

<div class="accordion" id="toc-accordion">
        <div class="accordion-item">
            {% for notebook in site.data.notebooks %}
                {% assign panelId = "panel" | append: forloop.index %}
                {% assign panelCollapseId = "panelCollapse" | append: forloop.index %}
                {% assign dataBsTarget = "#panelCollapse" | append: forloop.index %}
                <h2 class="accordion-header" id="{{ panelId }}">
                <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="{{ dataBsTarget }}" aria-expanded="true" aria-controls="{{ panelCollapseId }}">
                    {% assign notebookname = "Notebook " | append: notebook.number | append: " (" | append: notebook.date | append: ")" %}
                    <h2>
                        {% if notebook.title %}
                            {{ notebookname | append: ": " | append: notebook.title }}
                        {% else %}
                            {{ notebookname }}
                        {% endif %}
                    </h2>
                </button>
                </h2>
                <div id="{{ panelCollapseId }}" class="accordion-collapse collapse show" aria-labelledby="{{ panelId }}">
                <div class="accordion-body">
                    <p><i>{{ notebook.description }}</i></p>
                    <p><a href="{{ notebook.url }}" target="_blank">View full notebook</a></p>
                    <ul>
                        <li>panelId: {{ panelId }}</li>
                        <li>panelCollapseId: {{ panelCollapseId }}</li>
                        <li>dataBsTarget: {{ dataBsTarget }}</li>
                        {% for section in notebook.contents %}
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