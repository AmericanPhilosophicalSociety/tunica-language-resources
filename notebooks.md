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

<button id="expandCollapseButton" class="btn btn-primary" onClick="expandCollapse()">Expand/Collapse All</button>

<div class="btn-group" role="group" aria-label="Select organization by notebook or organization by subject heading" style="padding-bottom: .75rem;">
  <input type="radio" class="btn-check" name="btnradio" id="sortByNotebook" autocomplete="off" checked>
  <label class="btn btn-outline-primary" for="sortByNotebook" onClick="sortByNotebook()">Sort by Notebook</label>

  <input type="radio" class="btn-check" name="btnradio" id="sortBySubject" autocomplete="off">
  <label class="btn btn-outline-primary" for="sortBySubject" onClick="sortBySubject()">Sort by Subject Heading</label>
</div>

<div id="toc">
    {% include toc.html %}
</div>

<div id="toc-by-topic" style="display: none">
    {% include toc-by-topic.html %}
</div>

<script>
    // function toggleOrganization() {
    //     let button = document.getElementById("toggleTOC");
    //     let toc = document.getElementById("toc");
    //     let tocByTopic = document.getElementById("toc-by-topic");
    //     if (toc.style.display === "none") {
    //         toc.style.display = "block";
    //         tocByTopic.style.display = "none";
    //         button.innerHTML = "Sort by Subject Heading";
    //     } else {
    //         toc.style.display = "none";
    //         tocByTopic.style.display = "block";
    //         button.innerHTML = "Sort by Notebook";
    //     }
    // }\
    // TODO: consolidate into one function?
    function sortByNotebook() {
        let button1 = document.getElementById("sortByNotebook");
        let button2 = document.getElementById("sortBySubject");
        let toc = document.getElementById("toc");
        let tocByTopic = document.getElementById("toc-by-topic");
        
        toc.style.display = "block";
        tocByTopic.style.display = "none";
        button1.addClass("checked");
        button2.removeClass("checked");
    }
    function sortBySubject() {
        let button1 = document.getElementById("sortByNotebook");
        let button2 = document.getElementById("sortBySubject");
        let toc = document.getElementById("toc");
        let tocByTopic = document.getElementById("toc-by-topic");
       
        toc.style.display = "none";
        tocByTopic.style.display = "block";
        button1.removeClass("checked");
        button2.addClass("checked");
    }
    function expandCollapse() {
        // let accordion = document.getElementById("toc-accordion");
        // accordion.addClass("show");
        // document.getElementById("toc-accordion").addClass("open");
        // document.getElementById("toc-accordion").collapse("toggle");
        // for all accordion: addClass("open") or removeClass("open");
        const collapseElementList = document.querySelectorAll('.collapse');
        // console.log("collapseElementList: " + collapseElementList[5].outerHTML);
        const collapseList = [...collapseElementList].map(collapseEl => new bootstrap.Collapse(collapseEl));
        // console.log("collapseElementList: " + collapseList[5].outerHTML);
        // const collapseElementListShorter = [];
        // look for class accordion-button
        // collapsed: accordion-button collapsed
        // uncollapsed: accordion-button 

        // use show and hide methods?
        // https://getbootstrap.com/docs/5.2/components/collapse/

        // for (let i = 0; i < collapseElementList.length; i++) {
        //     if (collapseElementList[i].class == "accordion-collapse collapse") {
        //         // new bootstrap.Collapse(collapseElementList[i]);
        //         collapseElementListShorter.push(collapseElementList[i]);
        //     }
        // }
        // console.log("collapseElementList: " + collapseElementList[5].outerHTML + collapseElementList[1]);
        
        // const collapseList = [...collapseElementListShorter].map(collapseEl => new bootstrap.Collapse(collapseEl));
        // iterate through collapseElementList
        // if anything is currently closed, open it (how to check this?)
        // if not, iterate through again and close everything
    }
</script>