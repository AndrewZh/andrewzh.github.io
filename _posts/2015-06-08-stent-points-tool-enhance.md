---
layout: post
title: "JUK project: Report for June 8th"
category: Reports
tags: 
  - stent point
  - enhancements
  - JUK
  - "stent point,enhancements,JUK"
comments: true
share: true
published: true
mathjax: false
featured: false
---

### Achieved enhancements
Today I have finished implementing some easy but cosy features for the stent points generation tool.

###### From now user can:
1. Return to the previous frame.
2. Rollback changes in the current frame. It means there is a possibility to remove points one by one inside one frame.
3. Save points without terminating application (when stopping points are also saved).

### Tool's howto or hot keys you'll definitely need
In order to use all the features one needs to know the keys that call one or another command. Of course, there is nothing special in putting points as it's quite straigtforward: just click your mouse left button.
However, there are another a little trickier but still intuitive key to press to achive your goal. And here's the list of them:

##### Keys
1. _**m**_ - switching to malapposed points
2. _**a**_ - switching to apposed points
3. _**c**_ - switching to contained points
4. _**s**_ - switching to side-branch points
5. _**u**_ - switching to points with unknown status
6. _**w**_ - save currently selected points
7. _**z**_ - remove the latest point on the current frame (if frame is empty nothing is done)
8. _**p**_ - go to the previous frame if there is one
9. _**n**_ - go to the next frame if there is one
10. _**b**_ - terminate application: all the points are saved.


### Points colour classification
As you may have noticed there are several types of points. That is why each type is assigned a specific colour to be distinguished when switching types and displaying combined scenes (i.e. vessel surface, carpet view).
Here is the colour classification used in the tool:

##### Types
1. Unknown points (default ones) - yellow
2. Malapposed points - blue
3. Apposed points - red
4. Contained points - green
5. Side-branch points - magenta
