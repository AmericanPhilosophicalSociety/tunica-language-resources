---
layout: default
title: 'The Tunica Language Notebooks'
parallax: true
image:
  img_url: '/assets/img/tunica-notebook-3.jpg'
  img_alt: A stack of three blue notebooks. The top notebook has a Yale University logo and handwritten text reading "Tunica III".
  caption: Mary Haas's Tunica notebooks
  cssClass: 'notebook'
permalink: /notebooks/
---
# {{ page.title }}

In the 1930s, the last known speaker of the Tunica language, Sesostrie Youchigant, worked with the linguist Mary Haas to preserve information on the Tunica language for future generations. The stories, vocabularies, and deep cultural knowledge told by Youchigant and written down in notebooks by Haas form a rich resource that is playing a key role in the ongoing reawakening of the Tunica language.

Haas’s notebooks are housed at the American Philosophical Society Library and Museum. **Use the links below to view digitizations and transcriptions of these notebooks.** Contents can be sorted by notebook number or by theme. Click on any section title to view that page in the relevant notebook.

The notebooks viewer was built using a modified version of [EditionCrafter](https://editioncrafter.org/). You can also view scans of the notebooks in the [APS Digital Library](https://diglib.amphilsoc.org/islandora/object/text%3Amssmscoll94tunicanotebookswithtoc?=&sort_order=ASC&sort_by=title).

<!-- <div class="view-all-notebooks-container">
<a href="https://diglib.amphilsoc.org/islandora/object/text%3AMss.Ms.Coll.94_TunicaNotebooksWithTOC?=&sort_order=ASC&sort_by=title" target="_blank" class="no-decoration-link">
        <div class="view-all-notebooks" style="background-image: url(&quot;{{ 'assets/img/TunicaNotebook14-006.jpg' | relative_url }}&quot;);">
            <h2>View All Notebooks</h2>
        </div>
    </a>
</div> -->

<!-- {% include view-button.html
  text = "View all notebooks"
  url = "https://diglib.amphilsoc.org/islandora/object/text%3AMss.Ms.Coll.94_TunicaNotebooksWithTOC"
%} -->

<div class="toc-buttons">

<div class="btn-group button-left" role="group" aria-label="Select organization by notebook or organization by subject heading">
  <input type="radio" class="btn-check" name="btnradio" id="sortByNotebook" autocomplete="off" checked>
  <label class="btn btn-outline-primary" for="sortByNotebook" onClick="sortByNotebook()">Sort by Notebook</label>

  <input type="radio" class="btn-check" name="btnradio" id="sortBySubject" autocomplete="off">
  <label class="btn btn-outline-primary" for="sortBySubject" onClick="sortBySubject()">Sort by Subject Heading</label>
</div>

<button id="expandCollapseButton" class="btn btn-primary button-right" onClick="expandCollapse()">Expand/Collapse All</button>

</div>

<div id="toc" style="display: block">
    {% include toc.html %}
</div>

<div id="toc-by-topic" style="display: none">
    {% include toc-by-topic.html %}
</div>

<script>
    // TODO: consolidate into one function?
    function sortByNotebook() {
        let toc = document.getElementById("toc");
        let tocByTopic = document.getElementById("toc-by-topic");
        
        toc.style.display = "block";
        tocByTopic.style.display = "none";
    }
    function sortBySubject() {
        let toc = document.getElementById("toc");
        let tocByTopic = document.getElementById("toc-by-topic");
       
        toc.style.display = "none";
        tocByTopic.style.display = "block";
    }
    function expandCollapse() {
        // determine which version of the TOC is currently displayed
        let toc = document.getElementById("toc");
        let currentToc = ((toc.style.display == "block") ? toc : document.getElementById("toc-by-topic"));
        // within that TOC, find any collapsed elements
        const closedElementList = currentToc.querySelectorAll('.accordion-collapse.collapse:not(.show)');
        // if any collapsed elements, expand them
        if (closedElementList.length > 0) {
            // console.log("element 1: " + closedElementList[0].outerHTML);
            const closedList = [...closedElementList].map(collapseEl => new bootstrap.Collapse(collapseEl));
        } else {
            // else, collapse everything
            const openElementList = currentToc.querySelectorAll('.accordion-collapse.collapse.show');
            // console.log("open element 1: " + openElementList[0].outerHTML);
            const openList = [...openElementList].map(collapseEl => new bootstrap.Collapse(collapseEl));
        } 
    }
</script>