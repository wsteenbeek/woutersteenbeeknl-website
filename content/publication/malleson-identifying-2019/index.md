---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: Identifying the appropriate spatial resolution for the analysis of crime patterns
subtitle: ''
summary: ''
authors:
- Nick Malleson
- Wouter Steenbeek
- Martin A. Andresen
tags:
- '"Crime"'
- '"Background signal noise"'
- '"Census"'
- '"Criminology"'
- '"Graphs"'
- '"Similarity measures"'
- '"Source code"'
- '"Theft"'
categories: []
date: '2019-06-01'
lastmod: 2020-09-28T13:46:08+02:00
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
publishDate: '2020-09-28T11:46:07.826130Z'
publication_types:
- 2
abstract: 'Background: A key issue in the analysis of many spatial processes is the
  choice of an appropriate scale for the analysis. Smaller geographical units are
  generally preferable for the study of human phenomena because they are less likely
  to cause heterogeneous groups to be conflated. However, it can be harder to obtain
  data for small units and small-number problems can frustrate quantitative analysis.
  This research presents a new approach that can be used to estimate the most appropriate
  scale at which to aggregate point data to areas.   Data and methods: The proposed
  method works by creating a number of regular grids with iteratively smaller cell
  sizes (increasing grid resolution) and estimating the similarity between two realisations
  of the point pattern at each resolution. The method is applied first to simulated
  point patterns and then to real publicly available crime data from the city of Vancouver,
  Canada. The crime types tested are residential burglary, commercial burglary, theft
  from vehicle and theft of bike.  Findings: The results provide evidence for the
  size of spatial unit that is the most appropriate for the different types of crime
  studied. Importantly, the results are dependent on both the number of events in
  the data and the degree of spatial clustering, so a single ‘appropriate’ scale is
  not identified. The method is nevertheless useful as a means of better estimating
  what spatial scale might be appropriate for a particular piece of analysis.'
publication: '*PLOS ONE*'
# url_pdf: https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0218324
doi: 10.1371/journal.pone.0218324
url_code: https://github.com/nickmalleson/Multi-Scale-Error-Analysis
---
