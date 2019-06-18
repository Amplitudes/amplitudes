---
title: Converting from Schnetz f-alphabet to MZVs through weight 14
excerpt: Related paper and mathematica code.
header:
   teaser: CubeSpecialPoints.png
   overlay_color: "#5e616c"
   overlay_image: CubeSpecialPoints.png
   overlay_filter: .6
categories:
- software
tags:
- software
- f-alphabet
- MZV
- N=4 SYM
- planar
- mathematica
author: John_Joseph
pinned: true
---
{% include base_path %}

# Link:
Paper and machine readable expressions.
  * Paper: [The Cosmic Galois Group and Extended Steinmann Relations for Planar N=4 SYM Amplitudes](https://arxiv.org/abs/1906.07116)
  * [Conversion Code](https://arxiv.org/src/1906.07116v1/anc)

# Author(s):
Simon Caron-Huot, Lance J. Dixon, Falko Dulat, Matt von Hippel, Andrew J. McLeod, Georgios Papathanasiou

# Abstract:
We describe the minimal space of polylogarithmic functions that is required to express the six-particle amplitude in planar N=4 super-Yang-Mills theory through six and seven loops, in the NMHV and MHV sectors respectively. This space respects a set of extended Steinmann relations that restrict the iterated discontinuity structure of the amplitude, as well as a cosmic Galois coaction principle that constrains the functions and the transcendental numbers that can appear in the amplitude at special kinematic points. To put the amplitude into this space, we must divide it by the BDS-like ansatz and by an additional zeta-valued constant ρ. For this normalization, we conjecture that the extended Steinmann relations and the coaction principle hold to all orders in the coupling. We describe an iterative algorithm for constructing the space of hexagon functions that respects both constraints. We highlight further simplifications that begin to occur in this space of functions at weight eight, and distill the implications of imposing the coaction principle to all orders. Finally, we explore the restricted spaces of transcendental functions and constants that appear in special kinematic configurations, which include polylogarithms involving square, cube, fourth and sixth roots of unity

# Point of the Code:
> At many of these points, transcendental constants beyond MZVs appear, such as
> alternating sums and multiple polylogarithms evaluated at higher roots of unity.
> To study the coaction at these points, it is especially useful to work in terms
> of an f-alphabet, which makes the coaction structure of these constants manifest.

# See also:
O. Schnetz. [Computer program hyperlogprocedures](https://www.math.fau.de/person/oliver-schnetz/)
