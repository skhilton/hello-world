---
layout: default
title: adding to the site
parent: site maintenance
nav_order: 1
---

# Adding to the site

## Adding a new page

You add a new page by creating a new `*.md` with the following header:  
```
---
layout: default
title: <TITLE>
nav_order: <NAV ORDER>
has_children: <TRUE or default FALSE>
parent: <PARENT TITLE or default FALSE>
---
```

Navigation order refers to the order of the page in the navigation list.
For example, the page with `<NAV ORDER>=1` will be at the top of the list

## Adding to an existing page
