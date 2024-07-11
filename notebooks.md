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

{% for notebook in site.data.notebooks %}
  <p>
    Notebook {{ notebook.number }}
  </p>
  <ul>
  {% for section in notebook.contents %}
    <li>
        {{ section }}
    </li>
  {% endfor %}
  </ul>
{% endfor %}

<div class="accordion" id="accordionPanelsStayOpenExample">
  <div class="accordion-item">
    <h2 class="accordion-header" id="panelsStayOpen-headingOne">
      <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#panelsStayOpen-collapseOne" aria-expanded="true" aria-controls="panelsStayOpen-collapseOne">
        <h2>Notebook 1 (1993)</h2>
      </button>
    </h2>
    <div id="panelsStayOpen-collapseOne" class="accordion-collapse collapse show" aria-labelledby="panelsStayOpen-headingOne">
      <div class="accordion-body">
        <p>View notebook</p>
        <p>Heading</p>
        <p>Heading</p>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="panelsStayOpen-headingTwo">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#panelsStayOpen-collapseTwo" aria-expanded="false" aria-controls="panelsStayOpen-collapseTwo">
        <s>Accordion Item #2</s>
      </button>
    </h2>
    <div id="panelsStayOpen-collapseTwo" class="accordion-collapse collapse" aria-labelledby="panelsStayOpen-headingTwo">
      <div class="accordion-body">
        <strong>This is the second item's accordion body.</strong> It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="panelsStayOpen-headingThree">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#panelsStayOpen-collapseThree" aria-expanded="false" aria-controls="panelsStayOpen-collapseThree">
        Accordion Item #3
      </button>
    </h2>
    <div id="panelsStayOpen-collapseThree" class="accordion-collapse collapse" aria-labelledby="panelsStayOpen-headingThree">
      <div class="accordion-body">
        <strong>This is the third item's accordion body.</strong> It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
      </div>
    </div>
  </div>
</div>

<table class="table">
  <thead>
    <tr>
      <th scope="col">Notebook</th>
      <th scope="col">Year</th>
      <th scope="col">Details</th>
      <th scope="col">Expand/Collapse</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td scope="row">Notebook 1</td>
      <td>1933</td>
      <td></td>
      <td>
        <a class="btn btn-primary" data-toggle="collapse" href="#collapseExample" role="button" aria-expanded="false" aria-controls="collapseExample">
            Expand
        </a>
        </td>
    </tr>
    <tr>
      <td>
        Elicitation
        How the Tunica Got Their Flag
        Elicitation (Sept 7, 1933)
        Thunder Myth
        Notes on Noun Gender
      </td>
    </tr>
    <tr>
      <td scope="row">Notebook 2</td>
      <td>1933</td>
      <td></td>
      <td>TK</td>
    </tr>
    <tr>
      <td scope="row">Notebook 3</td>
      <td>1933</td>
      <td>Music</td>
      <td>TK</td>
    </tr>
  </tbody>
</table>


<div id="accordion">
  <div class="card">
    <div class="card-header" id="headingOne">
      <h5 class="mb-0">
        <button class="btn btn-link" data-toggle="collapse" data-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
          Notebook 1 (1933)
        </button>
      </h5>
    </div>
    <div id="collapseOne" class="collapse show" aria-labelledby="headingOne" data-parent="#accordion">
      <div class="card-body">
        Elicitation
      </div>
    </div>
  </div>

  <div class="card">
    <div class="card-header" id="headingTwo">
      <h5 class="mb-0">
        <button class="btn btn-link collapsed" data-toggle="collapse" data-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
          Notebook 2 (1933)
        </button>
      </h5>
    </div>
    <div id="collapseTwo" class="collapse" aria-labelledby="headingTwo" data-parent="#accordion">
      <div class="card-body">
        Elicitation
      </div>
    </div>
  </div>
  <div class="card">
    <div class="card-header" id="headingThree">
      <h5 class="mb-0">
        <button class="btn btn-link collapsed" data-toggle="collapse" data-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
          Notebook 3 (1933)
        </button>
      </h5>
    </div>
    <div id="collapseThree" class="collapse" aria-labelledby="headingThree" data-parent="#accordion">
      <div class="card-body">
        Auxiliary - added to infintive
      </div>
    </div>
  </div>
</div>


# Notebooks 1-4

## Notebook 1

Elicitation
How the Tunica Got Their Flag
Elicitation (Sept 7, 1933)
Thunder Myth
Notes on Noun Gender

## Notebook 2

Elicitation
The Story of Bayou de Glaise
Elicitation
The Tasks of Rabbit
Elicitation
The Origin of the Pole-Bean (first telling)
The Origin of Corn (first telling)
About Fire
How Eating Implements were made
How They Used to Cook
How Corn-meal was made
How Hominy was made
Flood Myth (first telling)

## Notebook 3

Auxiliary - added to infintive
Elicitation
William Ely Johnson
Elicitation
Numbers
The Tunica and the Spanish Defeat the Avoyelle
What they Used to Eat
How They Used to Cure Fever
How They Used to Shoot Ghosts
Elicitation
How They Used to Make Baskets
Old-Time Houses and Furniture
Types of Dances. Of the Choctaw and Koasati (in English)
Elicitation
The Three Owls
Elicitation

## Notebook 4

Elicitation
Paradigms
Elicitation
How They Used to Tan Hides
Elicitation
Woodpecker
Elicitation
A Hunting Trip Ends in Battle
Recording info (in English)
The Tunica Take Revenge
Recording info (in English)
A Choctaw Ball
How they Danced the Rabbit Dance
How they Danced the Bear Dance
Elicitation
The One-Eyed Indians
Elicitation

# Notebook 5: Music

## Notebook 5

Tunica Songs
Record No. 37 - Rabbit Dance Song
Record No. 38 - Rabbit Dance
Notes on Old-Time Instruments
Record No. 39 - Raccoon Dance - "Corn Dance"
Record No. 41 - Duck Dance
Record No. 42 - Chicken Dance
Record No. 43 - Bear Dance
Record No. 44 - Alligator Dance
Record No. 45 - After Midnight Dance
Record No. 46 - Two-heads Dance
Record No. 47 - Quail Dance
Record No. 48
Record No. 49 - Stealing Dance
Record No. 20 - Round Dance
Record No. 21
Record No. 22 - Round Dance Song
Record No. 23
Record No. 24 - Round Dance Song (cont.)
Record No. 13 - Round Dance Song (cont.)
Record No. 14 - Tunica Speech: The Thunder Myth
Record No. 1 - Alligator Dance
Record No. 2 - Alligator Dance
Dictaphone Record No. 36
Record No. 3 - Two Heads Dance
Dictaphone Record No. 36 (cont.)
Record No. 4 - Round Dance
Record No. 5 - Round Dance
Record No. 6 - Round Dance
Record No. 7
Record No. 8 - Coon Dance
Record No. 50 - Blue Heron Dance
Record No. 51 - Blue Heron Dance
Record No. 52 - Turtle Dance
Record No. 53 - Corn Dance
Record No. 54 - Bear Dance
Record No. 55 - Duck Dance
Record No. 56 - Round Dance
Record No. 57 - Round Dance (cont.)
Record No. 58 - Round Dance (cont.)
Record No. 59 - Round Dance (cont.)
Record No. 60 - Round Dance (cont.)
Record No. 61 - Round Dance (cont.)
Record No. 62 - Round Dance (cont.)
Record No. 63
Record No. 64 - Song of Owl Mammoth
Record No. 65 - Part of Tick Dance Song
Record No. 66
Record No. 14 - The Thunder Myth
Dance information

# Notebooks 6-9

## Notebook 6

Preamble - The Owl Mammoth
The Owl Mammoth
Preamble - Mammoths
Mammoths
Comparatives and Superlative Constructions
Tigre Blanc
Dew, Corn Shucking, Weaving
How They Used to Make Hats From Palmetto Leaves
Preamble - The Ahpasa Lamihta
The Ahpasa Lamihta
The Biloxi
The Origin of Indian Bayou
Preamble - How they Danced the Raccoon Dance
How They Danced the Raccoon Dance
On Catching Baby Deer
Enough
How and What They Used to Hunt
Crossed out page
Black bear
Sesostrie's Family
Elicitation
Preamble - The Lord Tests Rabbit Three Times (2nd Telling)
The Lord Tests Rabbit Three Times (2nd Telling)
Elicitation
Preamble - The Origins of the Pole-Bean (2nd telling)
The Origin of the Pole-Bean (2nd telling)
Elicitation
Choctaw Vocabulary
Animals
Deer and Turtle as Rivals
Owl Mammoth Translation

## Notebook 7

Preamble - Notes on Contraction in Tunica
Notes on Contraction in Tunica - Verb stems ending in a
Verb stems ending in i
Verb stems ending in u
Verb stems of the pattern C+V+h+V
Verb stems of the pattern C+V+C+V
Verb stems of the pattern C+V+V
Verb stems of the pattern C+V
Elicitation
Notes on Phonetics in connection with the Objectival Prefixes - Verb stems beginning with '
Verb stems beginning in h
Verb stems beginning in voiceless stops
Verb stems beginning in ablauts
Verb stems beginning in voiced consonants
Preamble - Thunder Myth
Thunder Myth
Preamble - Star Country
Star Country
A note on music
to be (auxiliary verb paradigm)
to lie (auxiliary verb paradigm)
to sit (auxiliary verb paradigm)
to cause (auxiliary verb paradigm)
to go (auxiliary verb paradigm)
to come (auxiliary verb paradigm)
Active verb endings

## Notebook 8

The Messanger of Death - preamble
The Messanger of Death
Le Juif Errant - preamble
Le Juif Errant
Solar Myth - preamble
Solar Myth
The Country Under the Water
Elicitation
A Bank Robbery - preamble
A Bank Robbery
Eliciation
The Night Owl
The Avoyelle Woman who Never Died
Elicitation
The Mounds Near Marksville
The Origin of Corn (second telling) preamble
The Origin of Corn (second telling)
The Flood Myth (second telling)
Sesostrie Dreams About a Rabbit
Elicitation
A saying
Ticlina
Elicitation
Beginning of 1934 Notes
The Creation of the Turtle
Elicitation
The Opposum and the Turtle
Elicitation

## Notebook 9

a
ä
e
i
ɔ
o
u
Elicitation
Body Parts
Elicitation
Verb Paradigms
Elicitation
Beginning of 1934 Notes

# Notebooks 10-11: Notes on Swanton's Vocabulary

## Notebook 10

Vowels a, ä, e     
h    
i    
k    
l    
n    
o    
p 

## Notebook 11

p (continued)    
r    
s    
š    
č    
t    
u    
w    
y

# Notebooks 12, 14-15

## Notebook 12

Continued from Notebook 9
Notes and Elicitation
The Solar Myth (2nd telling)
Addendum to How & What the Indians Used to Hunt
How They Made Baskets
About Fire
How They Tanned Hide
The Clawed Witch
The Origin of Bayou de Glaise (second telling)
Elicitation
On Catching Baby Deer
Elicitation
The Migration of Tunica
The Emergence of the Avoyelles
Notes and Questions

## Notebook 14

The Origin of Corn
The Singing Woman
Origin of the Tunica / The Tunica Fight the English
Elicitation
A Good Deed Forgotten
Elicitation
Face Painting and Dances
Elicitation
Ethnobotany
The Emergence of the Tunica
About Red River
Flint
Ethnobotany
Why the Tunica and Biloxi Became Friends - Notes
Why the Tunica and Biloxi Became Friends
Notes from C. Dorman
Quotes from S. Youchigant
Elicitation
Area languages
Notes

## Notebook 15

The Puppy That Saved His Master
How Flamant Came to be Bald-Headed
Elicitation
Snake or bite cure
Sun dance words
Solar Myth
Ball game (in English)
The Stone Witch
The Clawed Witch
Elicitation
Mobilian
Ethnobotany (in English)
Dances (in English)
Elicitation (Tunica) with interspersed Ethnobotany (English)
Story told by S's grandmother
Checking vocabulary
1938 Notes
The Drying Up of the Ocean
War with Pascagoula + Natchez
Numbers
Miscellaneous notes (in English)
Elicitation
Things still to be checked
About food (in English)
Elicitation
Notes (in English)