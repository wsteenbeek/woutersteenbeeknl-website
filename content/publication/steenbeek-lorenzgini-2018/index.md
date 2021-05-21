---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: 'lorenzgini: generalized Gini for sparse data situations'
subtitle: ''
summary: ''
authors:
- Wouter Steenbeek
tags: []
categories: []
date: '2018-01-01'
lastmod: 2020-09-28T13:46:11+02:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2020-09-28T11:46:10.745636Z'
publication_types:
- 0
abstract: lorenzgini is an R package that calculcates the standard Gini coefficient
  as well as the generalized coefficient, and plots Lorenz curves. The Lorenz plots
  show the line of maximal equality given the data.  The package builds on this paper
  in which Wim Bernasco and I wrote that the crime and place literature lacks a standard
  methodology for measuring and reporting crime concentration. We suggested that crime
  concentration be reported with the Lorenz curve and summarized with the Gini coefficient,
  and we proposed generalized versions of the Lorenz curve and the Gini coefficient
  to correct for bias when crime data are sparse (i.e., fewer crimes than places).  The
  proposed generalizations are based on the principle that the observed crime concentration
  should not be compared with perfect equality, but with maximal equality given the
  data. The generalizations asymptotically approach the original Lorenz curve and
  the original Gini coefficient as the number of crimes approaches the number of spatial
  units.
publication: ''
url_code: https://github.com/wsteenbeek/lorenzgini
---
