---
layout: post
title: "Milestones for Jena UK (June-July)"
modified: 
  - 2015-06-07T00:00:00.000Z
  - "Sun Jun 07 2015 03:00:00 GMT+0300 (MSK)"
  - "Sun Jun 07 2015 03:00:00 GMT+0300 (MSK),Sun Jun 07 2015 03:00:00 GMT+0300 (MSK)"
category: Milestones
tags: 
  - milestones
  - JUK
  - "milestones,JUK"
  - "milestones,JUK,milestones,JUK"
comments: true
share: true
published: true
mathjax: false
featured: false
---


#### Enhancing tool for stent points generation
1. returning to the previous frame
2. undo changes
3. saving points without termination
4. enhance termination

After this start implementing calculus

#### Major calculus tasks
1. Calculate volume of the following areas:
	1. Mallapposed
	2. Apposed
2. Providing carpet view:
	1. Calculate vessel contour length at fixed point
	2. Calculate stent contour length at fixed point
	3. Provide a 2D projection of points and contours
	4. Generate final view

### June

#### By June 11th
Enhance stent-point-generation tool

#### By June 20th
Implement following tasks:
- points area detection
- calculating points area intersecting or non-intersecting (depends on the point type) with inner vessel area

#### By June 27th
Implement volume function interpolation. Consequently, there will be an opportunity to caclulate volume.

### July

#### By July 4th
Implement stent and vessel contour length calculation. Previously implemented task on area detection should be used.

#### By July 18th
Implement carpet view without stent points simply providing circumference diagram using contour lengthes.

#### By July 25th
Implement points projection. Integrate into carpet view and test.
