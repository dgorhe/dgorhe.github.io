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

CLIP-seq gives us the RNA sequences bound by RNA-binding proteins in vivo using UV crosslinking followed by antibody pulldown(s) and sequencing. Many labs have contributed to CLIP-seq variants that make the detection of RNA species bound to RBPs more sensitive (iCLIP, eCLIP), more specific (easyCLIP, PAR-CLIP), and more multiplexed (SPIDR, ABC). Many methods have been developed to analyze this data (Skipper, CIMS, Piranha, PureCLIP, omniCLIP, etc) that aim to tell us: what information about RBP-binding behavior do we get from CLIP-seq? In particular, what information can we get from CLIP-seq that cannot be found by other methods? My work aims to address this question by looking at the distribution of crosslink spacing rather than the concentration of crosslinking events within a window.
