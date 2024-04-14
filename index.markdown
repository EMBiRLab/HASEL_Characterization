---
# Front matter. This is where you specify a lot of page variables.
layout: default
title:  "HASEL Actuator Design for Out-of-Plane Bending: A Parameteric Study of Planar Geometry"
date:   2023-06-16 03:03:01 -0400
description: >- # Supports markdown
  This is the main project page and the page used to demonstrate how this works with all of the options for the Front Matter present
show-description: false

# Add page-specifi mathjax functionality. Manage global setting in _config.yml
mathjax: true
# Automatically add permalinks to all headings
# https://github.com/allejo/jekyll-anchor-headings
autoanchor: false

# Preview image for social media cards
image:
  path: https://cdn.pixabay.com/photo/2019/09/05/01/11/mountainous-landscape-4452844_1280.jpg
  height: 100
  width: 256
  alt: Random Landscape

# Only the first author is supported by twitter metadata
authors:
  - name: Zachary Brei
    footnotes: 1
    email: breizach [at] umich.edu
    mailto: breizach@umich.edu
  - name: Chae Woo Lim
    # url: https://buildingatom.io
    email: chaewlim [at] umich.edu
    mailto: chaewlim@umich.edu
    footnotes: 1
  - name: Anneliese Ferguson
    email: annferg [at] umich.edu
    mailto: annferg@umich.edu
    footnotes: 2
  - name: Anvay A. Pradhan
    email: anvay [at] umich.edu
    mailto: anvay@umich.edu
    footnotes: 1
  - name: Varshni Vinayagam Sangeetha
    email: varshni [at] umich.edu
    mailto: varshni@umich.edu
    footnotes: 1
  - name: Xiangyun Bu
    email: xybu [at] umich.edu
    mailto: xybu@umich.edu
    footnotes: 1
  - name: Brent Usui
    email: busui [at] umich.edu
    mailto: busui@umich.edu
    footnotes: 3
  - name: Daniel B. Johnson
    email: dbjohn [at] umich.edu
    mailto: dbjohn@umich.edu
    footnotes: 1
  - name: Ram Vasudevan
    footnotes: 4
  - name: Talia Y. Moore
    footnotes: 4


# If you just want a general footnote, you can do that too.
# See the sel_map and armour-dev examples.
author-footnotes:
  1: Mechanical Engineering, University of Michigan
  2: Electrical Engineering, University of Michigan
  3: Biomedical Engineering, University of Michigan
  4: Robotics, University of Michigan
  5: Zachary Brei, Chae Woo Lim, and Anneliese Ferguson are co-first authors.

# links:
#   - icon: arxiv
#     icon-library: simpleicons
#     text: Arxiv HP
#     url: https://arxiv.org/
#   - icon: bi-map
#     icon-library: bootstrap-icons
#     text: SEL_Map Ex.
#     url: /project-pages/sel_map
#   - icon: bi-bezier2
#     icon-library: bootstrap-icons
#     text: ARMOUR Ex.
#     url: /project-pages/armour-dev
#   - icon: github
#     icon-library: simpleicons
#     text: Code
#     url: https://github.com/BuildingAtom/project-pages

# End Front Matter
---

{% include sections/authors %}
<!-- {% include sections/links %} -->

<!-- # Current Work In Progress -->

<!-- *TODO: adjust links above*

*TODO: add citation at end* -->
---

<div markdown="1" class="content-block grey justify no-pre">
# [Abstract](#abstract)

Soft robotic systems are promising for a wide range of applications from locomotion to manipulation.
In particular, fluidic dielectric elastomer actuators, such as Hydraulically Amplified Self-healing ELectrostatic (HASEL) actuators, demonstrate several compelling properties when compared to other soft robotic actuators such as lower power consumption, faster response times, and self-sensing capabilities.
Current HASEL actuator research has thoroughly characterized linear HASEL actuators, but there is a lack of geometric characterization for bending HASEL actuators.
This paper addresses this gap through the characterization of two important design parameters that affect out-of-plane bending of planar HASEL actuator designs.
In particular, a sinusoidal wave pattern is parameterized by the period length and the minimum channel width. 
The ratio of the period length to channel width is shown to be a good predictor for the curvature of the HASEL actuators when bending out-of-plane. 
The experimentally derived relationship is then used to demonstrate different grasp types for various objects.

<!-- <dic markdown="1" class="no-pre"> -->
<!-- ![](Sequence%2001_2.gif) -->
<!-- </div> -->
</div>

<div markdown="1" class="content-block grey justify no-pre">
# [Out-of-Plane Bending Motion](#overview)

By varying the heat-seal planar geometry, the out-of-plane bending performance is greatly affected. Shown below is a series of HASEL actuators, all with a channel width of \\(W_C = 5 mm\\), that have different period lengths. 

<p align="center">
  <img src="Sequence%2001_2.gif" width="100%" alt="animated" />
</p>

</div>


<div markdown="1" class="content-block grey justify no-pre">
# [Parameterizing Planar Heat-Seal Geometry of HASELs](#planar_geometry_of_HASELs)

![Diagram of two planar designs of bending HASEL actuators. The key parameters investigated are the period $T$ of the sine wave and the channel width \\(W_C\\), which describes the smallest width of the bending region of the HASEL actuator.](Fig2.jpg)

This paper focuses on determining the effects of different heat-seal patterns on the out-of-plane bending motion. 
We distinguish between the electrode (black) and the actuation (grey) portion of a HASEL actuator, shown in the figure above, where the actuation portion is the portion bending out-of-plane. 
We chose to use a sinusoidal profile for the actuator portion of the heat-seal. 
The sinusoid is parameterized by a period \\(T\\) and an amplitude \\(A\\). 
The valleys of the sinusoids are offset from the actuator centerline by a distance \\(W_C\\), which we refer to as the Channel Width. 
The sinusoid, and therefore bending portion of the actuator, has a length \\(L_X\\). 
The electrode portion has a length \\(L_E\\) and width \\(W\\). 
The total length of the HASEL actuator is therefore \\(L = L_X + L_E\\).
In this paper, we chose to explore the effect of varying the period \\(T\\) and channel width \\(W_C\\). 
Note that the total length of each actuator was kept constant, as were the dimensions of the electrode portion.
The dimensions of the strain limiting layer were also kept constant.
</div>

<!-- You can also make fullwidth embeds (this doesn't actually link to any video)
<div class="fullwidth">
<video controls="" style="background-color:black;width:100%;height:auto;aspect-ratio:16/9;"></video>
</div> -->

<div markdown="1" class="content-block grey justify no-pre">
# [Experimental Methods](#experimental_methods)

An initial sampling grid of 25 points were created with periods \\(T \in 10,12,15,20,30 \\) and channel widths \\(W_C \in 5,10,15,20,25 \\).
An actuator was made for each combination of period and channel width. 
Once initial results were obtained, six additional actuators were made near the largest measured curvature.
The additional combinations were \\( (T,W_C) \in (8.57,2.5),(8.57,5),(8.57,10),(10,2.5),(12,2.5),(15,2.5) \\).
<!-- To measure the curvature of an actuator, we attached six 3D printed markers to the strain limiting layer using a small amount of super glue.
Note that the markers were observed to have no effect on the overall bending performance of the actuators. 
A PS2-10-030-08 High Voltage Power Supply (Artimus Robotics, Boulder, CO) was used with a custom Python script to actuate the HASEL actuators.
A voltage of 8 kV was applied for three seconds, and powered off for five seconds, and then repeated 5 times per actuator.
The movements of the HASEL actuators were captured via a video camera. 
Images are extracted from the videos when the actuators are steady at their peak curvature during each three second actuation. 
The images are then cropped  -->
The data collection and analysis process is described in the paper.

<!-- *TODO: add experimental methods figure* -->
![](Fig3.jpg)

<!-- *TODO: add text describing experimental methods* -->
Shown in a) is a HASEL actuator with a period T=15 mm and channel width W_C=10 mm. Demonstrated in b) is the result of a circle fit (purple) on the markers (red) attached to the actuator. The marker height is a constant offset, which is subtracted to obtain a fit to the actuator curvature (orange).The results for a HASEL actuator with period T=30 mm and channel width W_C=25 mm are presented in c) and d).

<!-- *TODO: add videos of HASEL actuating* -->
</div>

<div markdown="1" class="content-block grey justify no-pre">
# [Results](#results)

<!-- *TODO: add 3D plot of individual data points?*  -->
The results of testing 31 actuators is shown below. 
Each black circle is the average of the five actuations for each actuator. 
From the results, it is clear that bending curvature varies with the heat-seal geometry. 
Higher curvatures were obtained with narrower channel widths, with a maximum observed at a channel width of 5 mm.
Actuators with a channel width of 2.5 mm experienced choking of the fluid flow from the electrode portion into the actuation portion, preventing out-of-plane bending. 
The period of the sinusoidal wave also shows variation. 
At channel widths of 15 mm and above, increased curvature is observed with increasing period length. 
At channel widths less than 15 mm, increased curvature is observed with decreasing period length. 
Maximum curvature is obtained at a period length of 10 mm.

![Optimal Ratio of 2:1](Fig4.jpg)


Further insight can be gained in the relationship between the two design parameters by considering the curvature versus the ratio \\(T : W_C\\) of the period to the channel width, as seen in the figure below.
Actuators with period lengths of 30 mm experience asymptotic behaviour with increasing ratio, resulting in slight bending deformation. 
Actuators with smaller period lengths exhibit peak curvature near period to channel width ratios of 2:1.

![Optimal Ratio of 2:1](Fig5.jpg)

<!-- *TODO: add text describing results* -->
</div>

<div markdown="1" class="content-block grey justify no-pre">
# [Conclusion](#conclusion)

The variation in bending caused by different combinations of period length and channel width can be harnessed to achieve various types of grasps. 
A series of dexterous grasping tests were performed to assess the range of objects that the bending HASEL actuators could lift, as shown in the figure below. 
Different combinations of HASEL actuators were combined to create different grasping modes.

Shown in a) is two HASEL actuators that exhibit medium to high curvature conducting a Palmar-Pinch grasp to hold a ping-pong ball. 
A Palmar-Pinch grasp was implemented for precise manipulation of the curved surface of the ping-pong ball. 
A combination of a high curvature HASEL actuator and a low curvature HASEL actuator was used to perform a power ring grasp on a cardboard tube, as depicted in b). 
To hold the out-of-plane curvature of a plastic cup in c), a precise pincer grasp was implemented using actuators of equal geometry. 
In d), a medium wrap grasp was created using high curvature HASEL actuators to wrap around a Rubik’s cube for stability. 
The grasping tests demonstrated the ability to generate different grasping types by varying the geometry of the HASEL actuators, depending on the need for power or precision.
![Different grasps types acheived using different HASEL actuator designs.](Fig6.jpg)
 
</div>

<div markdown="1" class="content-block grey justify">

# Citation

*TODO: add bibtex citation*

!-- ```bibtex
@article{nash51,
  author  = "Nash, John",
  title   = "Non-cooperative Games",
  journal = "Annals of Mathematics",
  year    = 1951,
  volume  = "54",
  number  = "2",
  pages   = "286--295"
}
``` --
</div>
