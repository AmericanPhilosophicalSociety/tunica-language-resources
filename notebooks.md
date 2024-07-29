---
layout: default
title: 'The Tunica Language Notebooks'
parallax: true
image:
  img_url: '/tunicanotebooks/assets/img/tunica-notebook-3.jpg'
  img_alt: A blue notebook with a Yale University logo and handwritten text reading "Tunica III".
  caption_url: 'https://diglib.amphilsoc.org/islandora/object/women-science-nd/'
  caption: Mary Haas's Tunica notebooks
---
# {{ page.title }}

In the 1930s, the last known speaker of the Tunica language, Sesostrie Youchigant, worked with the linguist Mary Haas to preserve information on the Tunica language for future generations. The stories, vocabularies, and deep cultural knowledge told by Youchigant and written down in notebooks by Haas form a rich resource that is playing a key role in the ongoing reawakening of the Tunica language.

You can view digitizations and transcriptions of these notebooks on the APS website, linked below.

{% include view-notebooks.html %}

You can also navigate the notebooks via their contents (below). Contents can be sorted by notebook number or by theme.

<button id="toggleTOC" onclick="toggleOrganization()" type="button" class="btn btn-primary btn-lg btn-block">Sort by Subject Heading</button>

<!-- <button id="expandCollapseButton" onClick="expandCollapse()">Expand/Collapse All</button> -->

<div id="toc">
    {% include toc.html %}
</div>

<div id="toc-by-topic" style="display: none">
    {% include toc-by-topic.html %}
</div>

<script>
    function toggleOrganization() {
        let button = document.getElementById("toggleTOC");
        let toc = document.getElementById("toc");
        let tocByTopic = document.getElementById("toc-by-topic");
        if (toc.style.display === "none") {
            toc.style.display = "block";
            tocByTopic.style.display = "none";
            button.innerHTML = "Sort by Subject Heading";
        } else {
            toc.style.display = "none";
            tocByTopic.style.display = "block";
            button.innerHTML = "Sort by Notebook";
        }
    }
</script>

<!-- <script>
    function expandCollapse() {
        // let panel = document.getElementById("panel1");
        // let button = document.getElementById("button1");
        // // button.aria-expanded = "true";
        // button.style.class = "accordion-button";
        // panel.class = "accordion-collapse collapse show";
        console.log("script runs");
        console.log("class of getElementById panelCollapse1: " + document.getElementById("panelCollapse1").class);
        document.getElementById("panelCollapse1").class = "accordion-collapse collapse show";
        console.log("class of getElementById panelCollapse1: " + document.getElementById("panelCollapse1").class);

        console.log("class of getElementById button1: " + document.getElementById("button1").class);
        document.getElementById("button1").class = "accordion-button";
        console.log("class of getElementById button1: " + document.getElementById("button1").class);
        // document.getElementById("button1").aria-expanded = "true";
    }
    let button = document.getElementById("expandCollapseButton");
    button.addEventListener("click", expandCollapse);
</script> -->

<!-- <script>
    $('.collapse').collapse()
</script> -->