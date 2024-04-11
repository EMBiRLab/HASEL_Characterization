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
    email: person [at] example.edu
    mailto: person@example.edu
    footnotes: 2
  - name: Anneliese Ferguson
    email: someemail@example.com
    footnotes: 3
  - name: Anvay A. Pradhan
    mailto: combined@example.com
    footnotes: 3
  - name: Varshni Vinayagam Sangeetha
  - name: Xiangyun Bu
  - name: Brent Usui
  - name: Daniel B. Johnson
  - name: Ram Vasudevan
  - name: Talia Y. Moore


# If you just want a general footnote, you can do that too.
# See the sel_map and armour-dev examples.
author-footnotes:
  1: Mechanical Engineering, University of Michigan
  2: Electrical Engineering, University of Michigan
  3: Biomedical Engineering, University of Michigan
  4: Robotics, University of Michigan
  5: Zachary Brei, Chae Woo Lim, and Anneliese Ferguson are co-first authors.

links:
  - icon: arxiv
    icon-library: simpleicons
    text: Arxiv HP
    url: https://arxiv.org/
  - icon: bi-map
    icon-library: bootstrap-icons
    text: SEL_Map Ex.
    url: /project-pages/sel_map
  - icon: bi-bezier2
    icon-library: bootstrap-icons
    text: ARMOUR Ex.
    url: /project-pages/armour-dev
  - icon: github
    icon-library: simpleicons
    text: Code
    url: https://github.com/BuildingAtom/project-pages

# End Front Matter
---

{% include sections/authors %}
{% include sections/links %}

# Current Work In Progress

*TODO: add emails and personal websites*

*TODO: adjust links above*
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

<div markdown="1" class="content-block grey justify">
# Topic inside of the content block

Lorem ipsum dolor sit amet Consectetur adipiscing elit Integer molestie lorem at massa.

![Alt Text](https://cdn.pixabay.com/photo/2019/09/05/01/11/mountainous-landscape-4452844_1280.jpg "Random Image")
</div>

# Topic outside of content block

![Alt Text](https://cdn.pixabay.com/photo/2019/09/05/01/11/mountainous-landscape-4452844_1280.jpg "Random Image")

Lorem ipsum dolor sit amet Consectetur adipiscing elit Integer molestie lorem at massa.

## This is how we can get the image at 100%

<div markdown="1" class="fullwidth">
![Alt Text](https://cdn.pixabay.com/photo/2019/09/05/01/11/mountainous-landscape-4452844_1280.jpg "Random Image")
</div>

## And this is how we can get the image closer

<div markdown="1" class="no-pre">
![Alt Text](https://cdn.pixabay.com/photo/2019/09/05/01/11/mountainous-landscape-4452844_1280.jpg "Random Image")
</div>

Lorem ipsum dolor sit amet Consectetur adipiscing elit Integer molestie lorem at massa.

<div markdown="1" class="cabin">
It's also possible to specify a new font for a specific section
</div>

<div markdown="1" class="jp">
## See? 1
</div>

And you can also <span class="cabin">change it in the middle</span>, though that's a bit more problematic for other reasons.

To specify fonts, just use Google Fonts and update `_data/fonts.yml`.
Any fonts you add as extra fonts at the bottom become usable fonts in the body of the post.

There are also tools to grab icons from other repos.
Just use the following:
{% include util/icons icon='github' icon-library='simpleicons' -%}
, and you'll be able to add icons from any library you have enabled that is supported.

This uses the liquid template engine for importing.
If you include the - at the start of end of such a line, it say to discard all whitespace before or after.
In order to keep the comma there, we added the -.
This is what happens:
{% include util/icons icon='github' icon-library='simpleicons' %}
, when you don't have it (notice the space).

And if you have mathjax enabled in `_config.yml` or in the Front Matter as it is here, you can even add latex:

$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$

You can also treat a section of text as a block, and use kramdown's block attribution methods to change fonts.
You can see at the end of this section in the markdown that I do just that
{: class="cabin"}

<div markdown="1" class="content-block grey justify">

# Citation

*TODO: add bibtex citation*

```bibtex
@article{nash51,
  author  = "Nash, John",
  title   = "Non-cooperative Games",
  journal = "Annals of Mathematics",
  year    = 1951,
  volume  = "54",
  number  = "2",
  pages   = "286--295"
}
```
</div>
