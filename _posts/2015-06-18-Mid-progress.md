---
layout: post
title: Mid progress on June 18th
category: Reports
tags: 
  - reports
  - JUK
  - "reports,JUK"
comments: true
share: true
published: true
mathjax: false
featured: false
---

Lately, I have been working on implementing the feature to retrieve image areas marked by user. This is a very important step in order to calculate the volume based on the several video frames.
In order to detect areas several algorithms were considered to be used.

##### Involved algorithms
1. Canny edge detection algorithm [(more here)](https://en.wikipedia.org/wiki/Canny_edge_detector)
2. Algorithm for finding contours implemented in OpenCV. It is applied to the output of the previous algorithm
3. Watershed image segmentation algorithm with markers [(more here)](https://en.wikipedia.org/wiki/Watershed_%28image_processing%29)

After considering which algorithms to use and learning 
