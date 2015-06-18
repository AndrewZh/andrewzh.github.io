---
layout: post
title: Mid progress on June 18th
category: Reports
tags: 
  - reports
  - JUK
  - "reports,JUK"
  - "reports,JUK,reports,JUK"
comments: true
share: true
published: true
mathjax: false
featured: false
---

#### Intro
Lately, I have been working on implementing the feature to retrieve image areas marked by user. This is a very important step in order to calculate the volume based on the several video frames.
In order to detect areas several algorithms were considered to be used.

##### Involved algorithms
1. Canny edge detection algorithm [(more here)](https://en.wikipedia.org/wiki/Canny_edge_detector)
2. Algorithm for finding contours implemented in OpenCV. It is applied to the output of the previous algorithm
3. Watershed image segmentation algorithm with markers [(more here)](https://en.wikipedia.org/wiki/Watershed_%28image_processing%29)

After considering which algorithms to use and knowing that all of them are ready to use (implemented in OpenCV library) the task seems really easy. Unfortunately, it did not appear to be so in practice. Not because of the difficulties with integration or anything else but because of the memory management problems.
As when I call a function to post-process the watershed algorithm result in the same manner as it is done [here](http://docs.opencv.org/master/d8/da9/watershed_8cpp-example.html) I get quite a disappointing message:

_octAreaDetection: malloc.c:2365: sysmalloc: Assertion `(oldtop == (((mbinptr) (((char *) &((av)->bins[((1) - 1) * 2])) - builtinoffsetof (struct mallocchunk, fd)))) && oldsize == 0) || ((unsigned long) (oldsize) >= (unsigned >long)((((builtinoffsetof (struct mallocchunk, fdnextsize))+((2 * (sizeof(sizet))) - 1)) & ~((2 * (sizeof(sizet))) - 1))) && ((oldtop)->size & 0x1) && ((unsigned long)oldend & pagemask) == 0)' failed.
Aborted_

Buggy code:

![]({{site.baseurl}}/images/code_june_18.png)

I am afraid I do not really understand how I can trigger any kind of error in such a small code snippet. Consequently, I have little idea on what can be changed to fix the error. So I am afraid I may be not meet the deadline for this task.

