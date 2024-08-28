**Next week:**
UUID (or APS ID?) for photo/video -> photos hyperlink

# General

+ get pages into folder to make directory easier to navigate / do something with config file?
+ get better crops/sizing for images in navigation cards

## CSS

+ sizing for figures - don't let them get too big
+ make fonts look better
+ more attractive button, Youchigant link etc

# Home page

+ tweak formatting for cards

# TOC

+ write script to get links for subject headings - WAIT ON THIS
+ fix CHARACTER PLACEHOLDER TK lines in yml

# Additional resources

+ make formatting look nice on landing page
+ how to format images in headers?

## Photographs

+ ideally, get caption below photos in carousel and maybe get rid of border. is this possible? probably not!

## Insights

+ more attractive header display w link back to main page - how should this look?

### Questions for CNAIR

+ more photos?
+ what kind of explanatory text?

# About the Language

+ *nicer looking landing page*
+ format title and read more
+ do something more w images? responsive sizing, center them?

# Oral Histories

+ add imgAlt field (or don't? just put images in page content?)
+ UUIDs for videos and photos? - this could help improve connection between videos and related images

## Questions for CNAIR

+ should this be called Community Commentaries? Video Interviews?
+ names for remaining two interview subjects
+ should videos be in a specific order?

# Mobile

+ Video player looks weird on mobile - get it to flex down if window is below a certain size
+ Why is header cut off on side?
+ Something bad happening w cards - they're covering text
+ Image galleries don't display full image
+ Insights: blog post size is not responsive


Modal on:
+ Photos in carousel?




ok, alternate plan

read in notebooks.yml
for each notebook, find contents section
for each line, convert from:

- How the Tunica Got Their Flag

to:

- title: How the Tunica Got Their Flag
      page: 14


https://diglib.amphilsoc.org/islandora/object/text%3A312180?page=

PID

then plug in page number

https://diglib.amphilsoc.org/node/233510?page=14

alter yml file
under each content, put page number? maybe I have to hand-code that?
could have the script add "- page: " under each item in contents

I already have a URL for each notebook loaded in
actually all I have to do is input a page number (with some script assistance?) and then I can build a link using notebook.url
and I think it makes sense to just do that from the toc template


# TO DO - SEPTEMBER
+ photo gallery
+ flexbox: make it look good on small laptop screen or phone