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
autoanchor: true

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
# [Planar Geometry of HASELs](#planar_geometry_of_HASELs)

*TODO: add figure of planar geometry*

*TODO: add text describing planar geometry*
</div>

<!-- You can also make fullwidth embeds (this doesn't actually link to any video)
<div class="fullwidth">
<video controls="" style="background-color:black;width:100%;height:auto;aspect-ratio:16/9;"></video>
</div> -->

<div markdown="1" class="content-block grey justify no-pre">
# [Experimental Methods](#experimental_methods)

*TODO: add experimental methods figure*

*TODO: add text describing experimental methods*

*TODO: add videos of HASEL actuating*
</div>

<div markdown="1" class="content-block grey justify no-pre">
# [Results](#results)

*TODO: add 3D plot of individual data points?* 

*TODO: add results plot of ratio*

*TODO: add text describing results*
</div>

<div markdown="1" class="content-block grey justify no-pre">
# [Conclusion](#conclusion)

*TODO: add different grasp figure*

*TODO: add text providing conclusion*
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
