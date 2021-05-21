---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Testing for similarity in area-based spatial patterns: Alternative methods\
  \ to Andresen's spatial point pattern test"
subtitle: ''
summary: ''
authors:
- Andrew P. Wheeler
- Wouter Steenbeek
- Martin A. Andresen
tags: []
categories: []
date: '2018-01-01'
lastmod: 2020-09-28T13:46:06+02:00
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
publishDate: '2020-09-28T11:46:06.166759Z'
publication_types:
- 2
abstract: Andresen's spatial point pattern test (SPPT) compares two spatial point
  patterns on defined areal units; it identifies areas where the spatial point patterns
  diverge and aggregates these local (dis)similarities to one global measure. We discuss
  the limitations of the SPPT and provide two alternative methods to calculate differences
  in the point patterns. In the first approach we use differences in proportions tests
  corrected for multiple comparisons. We show how the size of differences matters,
  as with large point patterns many areas will be identified by SPPT as statistically
  different, even if those differences are substantively trivial. The second approach
  uses multinomial logistic regression, which can be extended to identify differences
  in proportions over continuous time. We demonstrate these methods by identifying
  areas where pedestrian stops by the New York City Police Department are different
  from violent crimes for 2006–2016.
publication: '*Transactions in GIS*'
# url_pdf: 
url_preprint: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3111822
url_code: https://www.dropbox.com/s/j8bhyo5y994yyy0/Analysis_AltMethods_SPPT_Anony.zip?dl=0
doi: 10.1111/tgis.12341
---
