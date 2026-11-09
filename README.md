# Tunica Language Resources

This repository contains the source code for the [Tunica Language Resources](https://tunica-biloxi.amphilsoc.org) website, a collaboration between the [Center for Native and Indigenous Research](https://www.amphilsoc.org/library/CNAIR) and the [Center for Digital Scholarship](https://www.amphilsoc.org/center-digital-scholarship) at the American Philosophical Society.

## Project requirements:

- Jekyll 4.3.3

## Installation instructions

1. Install [Ruby](https://www.ruby-lang.org/en/downloads/) and [Jekyll](https://jekyllrb.com/docs/).
2. In your terminal, navigate to where you want to install the site, then clone this repo and move into the directory the process creates:

```
git clone git@github.com:AmericanPhilosophicalSociety/tunica-language-resources.git
cd tunica-language-resources
```

3. Install the Jekyll dependencies

```
bundle install
```

4. Run the site locally:

```
bundle exec jekyll serve --config _config_development.yml
```

Or if site is refreshing too slowly, try the following:

```
bundle exec jekyll serve --config _config_development.yml --incremental
```

5. Navigate to http://localhost:4000/ to preview the site.

## Build instructions

1. Run the following command:

```
bundle exec jekyll build --config _config.yml
```

2. Copy files from the _site directory into the appropriate directory on the static site server via WinSCP. You can safely delete (or not copy over) the thumbs.db file.

## URL changes

If site needs to be migrated to a new URL, that new URL must be set in _config_development. _config should stay the same unless adding a baseurl (or subpath).

Watch out for hard-coded URLs in the following places:

+ EditionCrafter manifests
+ notebooks.yml and notebooks-by-topic.yml (used to build the two TOC)
+ modal and modal-figure includes

## Notes

### EditionCrafter

The notebook display runs on a modified version of [EditionCrafter](https://editioncrafter.org/).

Note that the site will throw console errors about missing .xml files for individual pages and index.html files for whole notebooks. You can ignore these; EditionCrafter will still function without these backup files.

/assets/editioncrafter/editioncrafter.css and /assets/editioncrafter/editioncrafter.js were downloaded on 10/20/25 and modified to remove certain features from the EditionCrafter display. These will not reflect more recent updates to EditionCrafter.

See scripts and documentation for the EditionCrafter notebooks viewer [here](https://github.com/AmericanPhilosophicalSociety/tunica-scripts).

### Misc.

When adding a page with the same name as a subdirectory (e.g. notebooks.md and /notebooks), give the page an explicit permalink in its front matter, e.g.

```
permalink: /notebooks/
```
