---
layout: post
published: true
description: ""
headline: ""
modified: ""
categories: null
tags: ""
imagefeature: ""
mathjax: false
featured: false
comments: false
title: Contour detector result demo
---

## The Plots
This post is intended to demonstrate the results of the integrated (a little changed) contour detector. So here are the results:
![]({{site.baseurl}}/images/combined1.png)
![]({{site.baseurl}}/images/combined2.png)
![]({{site.baseurl}}/images/combined3.png)

## Note on results
As you may see the results may be a little distorted by the stent center _rings_ by side-branches and possibly by other factors not yet encountered. So next steps in detector improvement will be removing center _rings_, using information from previous and next frames (it may be a two step algorithm: 1st step - producing some result, 2nd step - enhancing the result).
However, now I will switch to integration of all the utilities into one program in order to make testing easier.