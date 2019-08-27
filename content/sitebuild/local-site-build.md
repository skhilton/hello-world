---
layout: default
title: local site build
parent: site maintenance
nav_order: 2
---

# local build for development

To set up the website, I followed the [`just-the-docs` documentation](https://pmarsceill.github.io/just-the-docs/).

After making changes, you can do a local build to check the changes before deploying to Github Pages.
Use the command `bundle exec jekyll serve`.

Note: there is some disconnect between the local Gem file and how Github Pages deploys.
Specifically, it seems that markdown files in subdirectories are included on the Github pages even if they are not included in the local build. 
