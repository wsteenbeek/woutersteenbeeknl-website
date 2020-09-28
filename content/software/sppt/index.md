---
title: "sppt: Spatial Point Pattern Test"
summary: "Implements several area-based tests that measure the degree of similarity at the local level between two spatial point patterns."
tags:
- sppt
- point pattern
date: 2018-03-22

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
 caption: Photo by Kelsey Knight on Unsplash
 focal_point: "Left"
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

[sppt](https://github.com/wsteenbeek/sppt) is an R package that implements several Spatial Point Pattern Tests. The first version of the package started with Martin Andresen's original [Spatial Point Pattern Test](http://www.sfu.ca/~andresen/spptest/spptest.html), but several other functions have been implemented since.

{{% alert note %}}
To install the package, follow the instructions on its [GitHub repository](https://github.com/wsteenbeek/sppt).
{{% /alert %}}

The tests in this package measure the degree of similarity at the local level between two spatial point patterns and is an area-based test. They are not used for the purpose of testing point patterns with the null hypotheses of random, uniform, or clustered distributions, but may be used to compare a particular point pattern with these distributions. One advantage of the tests is that they can be performed for a number of different area boundaries using the same original point datasets.

Apply these tests if you are fundamentally interested in the similarity of two (or more) spatial point patterns for a specified areal unit. Do incidences of some form of cancer have a similar spatial pattern to the locations of known risk factors? Does crime have a similar spatial pattern as drinking establishments? Is the spatial pattern of exports similar to the spatial pattern of imports? Additionally, this spatial point pattern test can be used in longitudinal contexts as well: Is the spatial pattern of crime this year similar to the spatial pattern of crime last year, or ten years ago?
