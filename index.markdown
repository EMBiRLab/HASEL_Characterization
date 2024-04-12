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
    email: person [at] example.edu
    mailto: person@example.edu
    footnotes: 1
  - name: Anneliese Ferguson
    email: someemail@example.com
    footnotes: 2
  - name: Anvay A. Pradhan
    mailto: combined@example.com
    footnotes: 1
  - name: Varshni Vinayagam Sangeetha
    footnotes: 1
  - name: Xiangyun Bu
    footnotes: 1
  - name: Brent Usui
    footnotes: 3
  - name: Daniel B. Johnson
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

# Current Work In Progress

*TODO: add emails and personal websites*

*TODO: adjust links above*

*TODO: add citation at end*
---

<div markdown="1" class="content-block grey justify no-pre">
# [Abstract](#abstract)

Soft robotic systems are promising for a wide range of applications from locomotion to manipulation.
In particular, fluidic dielectric elastomer actuators, such as Hydraulically Amplified Self-healing ELectrostatic (HASEL) actuators, demonstrate several compelling properties when compared to other soft robotic actuators such as lower power consumption, faster response times, and self-sensing capabilities.
% HASEL actuators have several benefits such as 
Current HASEL actuator research has thoroughly characterized linear HASEL actuators, but there is a lack of geometric characterization for bending HASEL actuators.
This paper addresses this gap through the characterization of two important design parameters that affect out-of-plane bending of planar HASEL actuator designs.
In particular, a sinusoidal wave pattern is parameterized by the period length and the minimum channel width. 
The ratio of the period length to channel width is shown to be a good predictor for the curvature of the HASEL actuators when bending out-of-plane. %, with an optimal ratio demonstrated.
The experimentally derived relationship is then used to demonstrate different grasp types for various objects.
</div>


<div markdown="1" class="content-block grey justify no-pre">
# [Planar Heat-Seal Geometry of HASELs](#planar_geometry_of_HASELs)

![Diagram of two planar designs of bending HASEL actuators. The key parameters investigated are the period $T$ of the sine wave and the channel width \\(W_C\\), which describes the smallest width of the bending region of the HASEL actuator.](Fig2.jpg)

This paper focuses on determining the effects of different heat-seal patterns on the out-of-plane bending motion. We chose to use a sinusoidal profile for the actuator portion of the heat-seal, shown in the figure above. The sinusoid is parameterized by a period \\(T\\) and an amplitude \\(A\\). The valleys of the sinusoids are offset from the actuator centerline by a distance \\(W_C\\), which we refer to as the Channel Width. The sinusoid, and therefore bending portion of the actuator, has a length \\(L_X\\). The electrode portion has a length \\(L_E\\) and width \\(W\\). The total length of the HASEL actuator is therefore \\(L = L_X + L_E\\).
</div>

<!-- You can also make fullwidth embeds (this doesn't actually link to any video)
<div class="fullwidth">
<video controls="" style="background-color:black;width:100%;height:auto;aspect-ratio:16/9;"></video>
</div> -->

<div markdown="1" class="content-block grey justify no-pre">
# [Experimental Methods](#experimental_methods)

*TODO: add experimental methods figure*
![Shown in a) is a HASEL actuator with a period T=15 mm and channel width W_C=10 mm. Demonstrated in b) is the result of a circle fit (purple) on the markers (red) attached to the actuator. The marker height is a constant offset, which is subtracted to obtain a fit to the actuator curvature (orange).The results for a HASEL actuator with period T=30 mm and channel width W_C=25 mm are presented in c) and d).](Fig3.jpg)

*TODO: add text describing experimental methods*

*TODO: add videos of HASEL actuating*
</div>

<div markdown="1" class="content-block grey justify no-pre">
# [Results](#results)

*TODO: add 3D plot of individual data points?* 

*TODO: add results plot of ratio*
![Optimal Ratio of 2:1](Fig5.jpg)

*TODO: add text describing results*
</div>

<div markdown="1" class="content-block grey justify no-pre">
# [Conclusion](#conclusion)

*TODO: add different grasp figure*
![So many grasps](Fig6.jpg)
 
*TODO: add text providing conclusion*
</div>

<div markdown="1" class="content-block grey justify">

# Citation

*TODO: add bibtex citation*

<!-- ```bibtex
@article{nash51,
  author  = "Nash, John",
  title   = "Non-cooperative Games",
  journal = "Annals of Mathematics",
  year    = 1951,
  volume  = "54",
  number  = "2",
  pages   = "286--295"
}
``` -->
</div>
