TOMORROW:

do something for photo display
colors on notebook buttons?
bring back the 'scroll up' button but in a way that doesn't break stuff

# General

+ *get pages into folder to make directory easier to navigate / do something with config file?*
+ change fonts - get from Brian and Paul
+ *get it on the server* / figure out workflow for getting it on the server

# TOC

+ write script to get links for subject headings - scrape web for subject headings, in those files find page numbers

# Additional Resources

## Photographs

+ **priority** - alternate photo display with info about subjects. this is waiting on photo metadata cleanup
+ integrate photo-subjects page onto actual site

# Oral Histories

+ add imgAlt field (or don't? just put images in page content?)
+ UUIDs for videos and photos? - this could help improve connection between videos and related images
+ should videos be in a specific order?

# Mobile / Small Screen View

+ what's going on with link size and centered text for 'see manuscripts/notebooks' cards?

# Links for TOC

https://diglib.amphilsoc.org/islandora/object/text%3A312180?page=

PID

then plug in page number

https://diglib.amphilsoc.org/node/233510?page=14


# Tunica Logo Colors

Orange color:

Hex:
#f89339

rgba(248,147,57,255)

Red:

#df2413

rgba(223,36,19,255)

Darker red:
#cf0c00

rgba(207,12,0,255)

# Video display

max-width 800px (or rem?)
padding 1rem

text should wrap under the video if it's overflowing



Speck photos:
https://diglib.amphilsoc.org/solr-search/content?search_api_fulltext=tunica&f%5B0%5D=collection_globalsearch%3AFrank%20G.%20Speck%20Papers&f%5B1%5D=genre%3APhotographs

Speck drawings:
https://diglib.amphilsoc.org/solr-search/content?search_api_fulltext=tunica&f%5B0%5D=collection_globalsearch%3AFrank%20G.%20Speck%20Papers&f%5B1%5D=genre%3ASketches


pick a few images to highlight- 5 or so from each collection?
link out to the rest

sort by collection / sort by people

do people have a node/stable ID?



people

Creator:
Speck
Haas
Neitzel

Subject:

names

or Creator/Photographer; Pictured/Depicted


some of these get a taxonomy term, others don't?

https://diglib.amphilsoc.org/solr-search/content?search_api_fulltext=tunica&f%5B0%5D=person_globalsearch%3APierite%2C%20Joseph%2C%20Jr.

vs

https://diglib.amphilsoc.org/taxonomy/term/17895

https://diglib.amphilsoc.org/taxonomy/term/17894


include custom link for Speck - separate photos he took and photos he appears in
AND narrow down to only tunica photos

same for Neitzel?


height="315" width="560"


how to make this look unique/like its own distinct project, not just a WIS clone?

come up with some new design for navcards
make it a square, be more deliberate w image selection, maybe make text opaque?

play around w design on 'notebooks' page - something with button colors
surprising 'view all notebooks' button

surprising 'view all manuscripts' button

could change: size, have an interesting texture/background from a project-related image, border from youchigant image?

images to use:
still from the oral histories
Speck drawings
notebooks (cropped)
Tunica alphabet (cropped)



consistently sized image thumbnails along the top bar. have a few pixels between them but don't have them spaced out so much
cut it down to like a square from the middle of the image?
make a consistently sized box below this - max-width 100%, height can be anything
within that, image has a max width of 100% and set a max height in pixels to keep it from getting too big?
below the image, print some text: its title (hyperlinked) and description, maybe eventually some info about the people displayed