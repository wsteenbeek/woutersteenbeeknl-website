---
title: "lorenzgini"

summary: "Calculates the standard Gini coefficient as well as the generalized coefficient, and plots Lorenz curves. The Lorenz plots show the line of maximal equality given the data."

date: 2018-03-12

tags:
- crime concentration
- crime pattern

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
 caption: Photo by Austin Distel on Unsplash
 focal_point: "Bottom"
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

[lorenzgini](https://github.com/wsteenbeek/lorenzgini) is an R package that calculcates the standard Gini coefficient as well as the generalized coefficient, and plots Lorenz curves. The Lorenz plots show the line of maximal equality given the data.

The package builds on [this paper](https://doi.org/10.1007/s10940-016-9324-7) in which Wim Bernasco and I wrote that the crime and place literature lacks a standard methodology for measuring and reporting crime concentration. We suggested that crime concentration be reported with the Lorenz curve and summarized with the Gini coefficient, and we proposed generalized versions of the Lorenz curve and the Gini coefficient to correct for bias when crime data are sparse (i.e., fewer crimes than places).

The proposed generalizations are based on the principle that the observed crime concentration should not be compared with perfect equality, but with maximal equality given the data. The generalizations asymptotically approach the original Lorenz curve and the original Gini coefficient as the number of crimes approaches the number of spatial units.

{{% alert note %}}
To install the package, follow the instructions on its [GitHub repository](https://github.com/wsteenbeek/lorenzgini).
{{% /alert %}}

The package goes a bit beyond the method in the published paper:

- In footnote 3 of our paper we stated that we ignored the bias in the standard Gini because the bias is small in exactly the situations that we were addressing: when # units of analysis is large. However, if there are only a few crimes (and for example all of which are located in one unit), the generalized gini will have quite some bias. In the package, we now also correct for this (using the function argument `unbiased`).

- Instead of the jackknife procedure we briefly discuss in the paper, a bootstrap procedure is implemented to calculate confidence intervals of the Gini. Our reasoning is that the jackknife only leads to a variance that can be used to calculate a standard error, but confidence intervals based on jackknife’s s.e. assume a normal distribution which is very often not the case. Bootstrapping gives correct (parametric or non-parametric) confidence intervals, although the usual caveats apply for small counts. Various options are possible, leveraging the `boot` package. Note that one can also automatically plot the distribution of the bootstrap-simulated Ginis.

- The Lorenz plot can be automatically rescaled. This could be more useful when comparing two crime types than the original plots (Figure 3 and Figure 5, right-hand side) in the paper.
