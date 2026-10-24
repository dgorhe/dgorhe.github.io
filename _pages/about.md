---
layout: about
title: about
permalink: /
subtitle: PhD Candidate, Jovanovic Lab · Columbia University

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: true
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I am a PhD candidate in the lab of Marko Jovanovic working on modeling crosslinking and immunoprecipitation sequencing (CLIP-seq) data using stochastic processes and mixture models.

CLIP-seq gives us the RNA sequences bound by RNA-binding proteins (RBPs). Many labs have developed CLIP-seq variants that improve sensitivity (iCLIP, eCLIP), specificity (easyCLIP, PAR-CLIP), and throughput (SPIDR, ABC). Analysis methods like Skipper, CIMS, Piranha, PureCLIP, omniCLIP, etc aim to parse this data to tell us: which RBPs are binding to which genes more than background. However, I would argue these methods don't yield much information unique to CLIP-seq data. We often find ourselves using other methods like cryo-EM to validate the claims from CLIP-seq data. My work aims to address this gap by looking at distribution of the crosslink spacing rather than the concentration of crosslinking events within a window.
