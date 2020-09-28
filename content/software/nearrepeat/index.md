---
title: "NearRepeat"
summary: "Uses the (Monte Carlo permutation based) Knox test for space-time clustering to quantify the spatio-temporal association between events."
tags:
- crime pattern
- point pattern
- spatio-temporal
date: 2019-10-12

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
 caption: Photo by Jayden Wong on Unsplash
 focal_point: Smart
 preview_only: true

links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/WouterSteenbeek
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

[NearRepeat](https://github.com/wsteenbeek/NearRepeat) is an R package uses the Knox test for space-time clustering to quantify the spatio-temporal association between events. In criminology, this test has been used to identify people and locations that are at disproportionate risk of victimization. Of interest is often not only the ‘same repeat’ victims (people or locations that after a first crime event, are targeted again within a short period thereafter), but also the ‘near repeat’ victims: **nearby** people or locations that are victimized within a short period after the first crime. For more information, see for example the [JDI Analysis Brief](http://www.ucl.ac.uk/jdibrief/analysis/repeat_victimisation).

{{% alert note %}}
To install the package, follow the instructions on its [GitHub repository](https://github.com/wsteenbeek/NearRepeat).
{{% /alert %}}

Several other options exist but have drawbacks:

-   [Prof. Jerry Ratcliffe’s](http://www.jratcliffe.net/software/) / [Temple University’s](http://www.cla.temple.edu/center-for-security-and-crime-science/projects/#near-repeat-calculator) Near Repeat calculator only works on Windows (and needs admin rights to execute and write files). It seems this software mislabels the rows and columns of its output files, which may lead to erroneous conclusions.

-   the free [JDI Near Repeat Toolkit](http://www.ucl.ac.uk/jill-dando-institute/research/research-groups/geo-crime/near_repeat_toolkit) also only works on Windows. However it is not actively supported and does not run on Windows 10.

-   the R package [surveillance](https://cran.r-project.org/package=surveillance) has implemented the `knox()` function, but this only works for a single spatial distance and temporal distance, whereas the current package also works with multiple bands of spatial and temporal distances, as well as same repeat analysis.

Note that in parallel with the development of the code here, Toby Davies has developed an alternative implementation in Python, which can be found [here](https://github.com/tobydavies/NearRepeat). We have collaborated on some of the accompanying materials and reviewed each other’s code, and as far as we are aware the two implementations should give identical results.
