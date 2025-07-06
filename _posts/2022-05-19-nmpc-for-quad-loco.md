---
title: Nonlinear Model Predictive Control for Quadrupedal Locomotion Using Second-Order Sensitivity Analysis
description: ICRA 2022 - 6th Full-Day Workshop on Legged Robots
layout: distill
published: true
date: 2022-05-19 14:44:33
img: /assets/img/kang2021nonliner/teaser.png
permalink: /nmpc-for-quad-loco/
tags: [robotics, arxiv]
categories: publication
authors:
  - name: Dongho Kang
    url: "https://donghok.me/"
    affiliations:
      name: CRL<d-footnote>Computational Robotics Lab.</d-footnote>, ETH Zurich
  - name: Flavio De Vintenti
    affiliations:
      name: CRL, ETH Zurich
  - name: Stelian Coros
    url: "http://crl.ethz.ch/"
    affiliations:
      name: CRL, ETH Zurich
bibliography:
---

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
      <img class="img-fluid" src="{{ '/assets/img/kang2021nonlinear/teaser.png' | relative_url }}" alt="" title="teaser"/>
  </div>
</div>

<br>

# Abstract

We present a versatile nonlinear model predictive control (NMPC) formulation for quadrupedal locomotion. 
Our formulation jointly optimizes a base trajectory and a set of footholds over a finite time horizon based on simplified dynamics models. 
We leverage second-order sensitivity analysis and a sparse Gauss-Newton (SGN) method to solve the resulting optimal control problems. 
We further describe our ongoing effort to verify our approach through simulation and hardware experiments. 
Finally, we extend our locomotion framework to deal with challenging tasks that comprise gap crossing, movement on stepping stones, and multi-robot control. 

**Paper: [[ArXiv](https://arxiv.org/abs/2207.10465)]** 

-----

# Supplementary Video

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/BrJSRlAJaX4" allowfullscreen></iframe>
</div>

-----

# Presentation

Video presentation at ["ICRA 2022 - 6th Full-Day Workshop on Legged Robots"](https://leggedrobots.org/).

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/CGtzHkMmNuY" allowfullscreen></iframe>
</div>

-----

# Demo

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/J9GfVgz80lk" allowfullscreen></iframe>
</div>

<br>

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/D99qXOs9uQs" allowfullscreen></iframe>
</div>

<br>

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/rUv4jwwKFiY" allowfullscreen></iframe>
</div>

<br>

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/NCCBZf-Nuas" allowfullscreen></iframe>
</div>

-----

# Bibtex

{% highlight txt %}
@misc{kang2022nonlinear,
  title={Nonlinear Model Predictive Control for Quadrupedal Locomotion Using Second-Order Sensitivity Analysis}, 
  author = {Kang, Dongho and De Vincenti, Flavio and Coros, Stelian},
  url = {https://arxiv.org/abs/2207.10465},
  year={2022},
  eprint={2207.10465},
  archivePrefix={arXiv},
  primaryClass={cs.RO},
}
{% endhighlight %}

-----

# Acknowledgment

This work has received funding from the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (grant agreement No. 866480.)
