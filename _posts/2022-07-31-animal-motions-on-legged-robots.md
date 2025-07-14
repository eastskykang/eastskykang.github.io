---
title: Animal Motions on Legged Robots Using Nonlinear Model Predictive Control
description: IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS 2022)
layout: distill
published: true
date: 2022-07-31 15:12:33
img: /assets/img/kang2022animal/kang2022animal.png
permalink: /animal-motions-on-legged-robots/
tags: [robotics, conference]
categories: publication
authors:
  - name: Dongho Kang
    url: "https://donghokang.net/"
    affiliations:
      name: CRL<d-footnote>Computational Robotics Lab.</d-footnote>, ETH Zurich
  - name: Flavio De Vintenti
    affiliations:
      name: CRL, ETH Zurich
  - name: Naomi C. Adam
    affiliations:
      name: LMB<d-footnote>Laboratory for Movement Biomechanics</d-footnote>, ETH Zurich
  - name: Stelian Coros
    url: "http://crl.ethz.ch/"
    affiliations:
      name: CRL, ETH Zurich
bibliography:
---

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
      <img class="img-fluid" src="{{ '/assets/img/kang2022animal/kang2022animal.png' | relative_url }}" alt="" title="teaser"/>
  </div>
</div>

<br>

# Abstract

This work presents a motion capture-driven locomotion controller for quadrupedal robots that replicates the non-periodic footsteps and subtle body movement of animal motions. 
We adopt a nonlinear model predictive control (NMPC) formulation that generates optimal base trajectories and stepping locations. By optimizing both footholds and base trajectories, our controller effectively tracks retargeted animal motions with natural body movements and highly irregular strides. 
We demonstrate our approach with prerecorded animal motion capture data. In simulation and hardware experiments, our motion controller enables quadrupedal robots to robustly reproduce fundamental characteristics of a target animal motion regardless of the significant morphological disparity.

**Paper: [[IEEE Xplore](https://ieeexplore.ieee.org/document/9981945)]** &emsp; **Open access: [[ETH Research Collection](https://www.research-collection.ethz.ch/handle/20.500.11850/589749)]**

-----

# Supplementary Video

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/TVV_GcNZ0Ts" allowfullscreen></iframe>
</div>

-----

# Presentation

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/nv2VcuxtL4s" allowfullscreen></iframe>
</div>

-----

# Bibtex

{% highlight txt %}
@inproceedings{kang2022animal,
  title={Animal Motions on Legged Robots Using Nonlinear Model Predictive Control}, 
  author={Kang, Dongho and De Vincenti, Flavio and Adami, Naomi C. and Coros, Stelian},
  booktitle={2022 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)}, 
  pages={11955-11962},
  year={2022},
  organization={IEEE},
  doi={10.1109/IROS47612.2022.9981945}
}
{% endhighlight %}

-----

# Acknowledgment

This work has received funding from the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (grant agreement No. 866480.) The ethics have been approved by the veterinary authorities of the canton Z&uuml;rich.