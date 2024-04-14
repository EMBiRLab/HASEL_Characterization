---
# Front matter. This is where you specify a lot of page variables.
layout: default
title:  "HASEL Actuator Design for Out-of-Plane Bending: A Parametric Study of Planar Geometry"
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

By varying the heat-seal planar geometry, the out-of-plane bending performance is greatly affected.
The HASEL actuators are composed of inextensible material with a stiffer layer on one side of the shell.
The difference in stiffnesses results in uneven bending during actuation and curvature is induced.
Shown below is a series of HASEL actuators, all with identical channel width \\(W_C = 5 mm\\), but different period lengths. 
Actuation is also shown to be repeatable.

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
Two actuators were made for each combination of period and channel width.
The HASEL actuators were manufactured by heat-sealing sheets Biaxially-Oriented Polypropylene (BOPP) in a clamshell heat press with an aluminum die in the shape of the desired sinusoidal profile.
After heat-sealing, a stiffer strain-limiting layer was attached, carbon paint electrode was applied, and a consistent volume fraction of fluid was injected into the cavity.
To determine the curvature of each actuator, six 3D printed markers were added to the strain-limiting layer.
During actuation, each HASEL actuator was recorded and the position with maximum curvature was extracted.
Using image analysis software, the markers were fit to a circle.
The height of the markers was then subtracted from the radius of the circle to obtain the curvature of each actuator.
Once initial results were obtained, six additional actuators were made near the largest measured curvature.
The additional combinations were \\( (T,W_C) \in (8.57,2.5),(8.57,5),(8.57,10),(10,2.5),(12,2.5),(15,2.5) \\).
<!-- To measure the curvature of an actuator, we attached six 3D printed markers to the strain limiting layer using a small amount of super glue.
Note that the markers were observed to have no effect on the overall bending performance of the actuators. 
A PS2-10-030-08 High Voltage Power Supply (Artimus Robotics, Boulder, CO) was used with a custom Python script to actuate the HASEL actuators.
A voltage of 8 kV was applied for three seconds, and powered off for five seconds, and then repeated 5 times per actuator.
The movements of the HASEL actuators were captured via a video camera. 
Images are extracted from the videos when the actuators are steady at their peak curvature during each three second actuation. 
The images are then cropped  -->
A more thorough manufacturing, data collection, and analysis process is described in the paper.

<!-- *TODO: add experimental methods figure* -->
![](Fig3.jpg)

<!-- *TODO: add text describing experimental methods* -->
Shown in a) is a HASEL actuator with a period T=15 mm and channel width W_C=10 mm. Demonstrated in b) is the result of a circle fit (purple) on the markers (red) attached to the actuator. The marker height is a constant offset, which is subtracted to obtain a fit to the actuator curvature (orange).The results for a HASEL actuator with period T=30 mm and channel width W_C=25 mm are presented in c) and d).

<!-- *TODO: add videos of HASEL actuating* -->
</div>

<div markdown="1" class="content-block grey justify no-pre">
# [Results](#results)

<!-- *TODO: add 3D plot of individual data points?*  -->
Each period and channel width were plotted against the experimentally determined maximum curvature.
The result was a 3D plot of the 31 actuators as shown below.
Each black circle is the average of the five actuations for each actuator. 
The plots show that bending curvature varies considerably with the heat-seal geometry. 
Higher curvatures were obtained with narrower channel widths, with a maximum observed at a channel width of 5 mm.
Actuators with a channel width of 2.5 mm experienced choking of the fluid flow from the electrode portion into the actuation portion, preventing out-of-plane bending. 
The period of the sinusoidal wave also shows variation.
At channel widths of 15 mm and above, increased curvature is observed with increasing period length. 
At channel widths less than 15 mm, increased curvature is observed with decreasing period length. 
Maximum curvature is obtained at a period length of 10 mm.

![Optimal Ratio of 2:1](Fig4.jpg)

A curvature ratio of period to the channel width \\(T : W_C\\) was defined to better understand the relationship between the two design parameters and allow for generalization of the results.
The curvature was plotted versus this ratio, seen in the figure below.
Actuators with period lengths of 30 mm experience only slight bending as increasing ratio results in asymptotic curvature.
Actuators with smaller period lengths, however, exhibit a peak curvature near period to channel width ratios of 2:1.
This holds for several different sets of period and channel width values.
Therefore, we propose that more than the particular values of period or channel width, the ratio is the important factor affecting the curvature of a planar HASEL actuator.

![Optimal Ratio of 2:1](Fig5.jpg)

<!-- *TODO: add text describing results* -->
</div>

<div markdown="1" class="content-block grey justify no-pre">
# [Conclusion](#conclusion)

This paper characterizes the effect of the heat-seal profile geometry on the bending of HASEL actuators.
Thirty-one different period and channel width combinations were manufactured.
The curvature of the actuators was measured through image processing and its relation to the geometric parameters was identified.
Higher curvature was generally associated with narrower channel widths, with a lower bound determined by choked fluid flow.
An optimal period to channel width ratio of 2:1 is identified for maximum curvature.

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

# [Citation](#citation)
This project was completed as a collaboration between the Evolution and Motion of Biology and Robotics (EMBiR) Lab and the Robotics and Optimization for Analysis of Human Motion (ROAHM) Lab at University of Michigan - Ann Arbor.
<!-- *TODO: add bibtex citation* -->

<span style="color:red">
@article{brei2024HASEL,

<span style="color:red">
  author={Brei, Zachary and Lim, Chae Woo and Ferguson, Annie and Pradhan, Anvay A. and Sangeetha, Varshni Vinayagam and Bu, Xiangyun and Usui, Brent and Johnson, Daniel B. and Vasudevan, Ram and Moore, Talia Y.},

  <span style="color:red">
  journal={IEEE RoboSoft 2024}, 

  <span style="color:red">
  title={ HASEL Actuator Design for Out-of-Plane Bending: A Parametric Study of Planar Geometry}, 
  year={2024},

  <span style="color:red">
  keywords={Soft Sensors and Actuators; Soft Robot Materials and Design;
      Soft Robot Applications}

  <span style="color:red">
  doi={[forthcoming]}

<span style="color:red">
}
<!-- </div> -->
