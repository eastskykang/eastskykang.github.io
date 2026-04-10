---
title: "Walk Like Dogs: Learning Steerable Imitation Controllers for Legged Robots from Unlabeled Motion Data"
description: ArXiv
layout: distill
published: true
date: 2025-07-02 22:39:00
img: /assets/img/kang2025learning/teaser.jpg
permalink: /learning-steerable-imitation-controllers/
tags: [robotics, character animation]
categories: publication
authors:
  - name: Dongho Kang
    url: "https://donghokang.net/"
    affiliations:
      name: CRL<d-footnote>Computational Robotics Lab.</d-footnote>, ETH Zurich
  - name: Jin Cheng
    url: "https://jin-cheng.me/"
    affiliations:
      name: CRL, ETH Zurich
  - name: Fatemeh Zargarbashi
    url: "https://fzargarbashi.github.io/"
    affiliations:
      name: CRL, ETH Zurich
  - name: Taerim Yoon
    affiliations:
      name: RILAB<d-footnote>Robot Intelligence Lab.</d-footnote>, Korea University
  - name: Sungjoon Choi
    url: "https://sites.google.com/view/sungjoon-choi/personal"
    affiliations:
      name: RILAB, Korea University
  - name: Stelian Coros
    url: "http://crl.ethz.ch/people/coros/index.html"
    affiliations:
      name: CRL, ETH Zurich
bibliography:
---

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
      <img class="img-fluid" src="{{ '/assets/img/kang2025learning/teaser.jpg' | relative_url }}" alt="" title="teaser"/>
  </div>
</div>

<br> 

# Abstract

We present an imitation learning framework that extracts distinctive legged locomotion behaviors and transitions between them from unlabeled real-world motion data. By automatically discovering behavioral modes and mapping user steering commands to them, the framework enables user-steerable and stylistically consistent motion imitation. Our approach first bridges the morphological and physical gap between the motion source and the robot by transforming raw data into a physically consistent, robot-compatible dataset using a kino-dynamic motion retargeting strategy. This data is used to train a steerable motion synthesis module that generates stylistic, multi-modal kinematic targets from high-level user commands. These targets serve as a reference for a reinforcement learning controller, which reliably executes them on the robot hardware. In our experiments, a controller trained on dog motion data demonstrated distinctive quadrupedal gait patterns and emergent gait transitions in response to varying velocity commands. These behaviors were achieved without manual labeling, predefined mode counts, or explicit switching rules, maintaining the stylistic coherence of the data.

**Open access: [[ArXiv](https://arxiv.org/abs/2507.00677)]**

-----

# Supplementary Video

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/DukyUGNYf5A" allowfullscreen></iframe>
</div>  

-----

# Demos

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/kang2025learning/sit-pace-sit.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/kang2025learning/spin.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/kang2025learning/gallop.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true  %}
    </div>
</div>
<div class="caption">
    Prerecorded dog motion sequences to a real-world robot: <i>Sit-pace-sit</i> (first), <i>Spin</i> (second) and <i>Gallop</i> (third)
</div>

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/kang2025learning/transitions.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true %}
    </div>
</div>
<div class="caption">
    <i>Unitree Go2</i> robot adaptively changing its gait pattern based on the forward velocity command.
</div>

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/kang2025learning/steerable-locomotion.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true %}
    </div>
</div>
<div class="caption">
    <i>Unitree Go2</i> robot navigating freely across a grass field in response to joystick commands.
</div>

-----

# Bibtex

{% highlight txt %}
@misc{kang2026walklikedogs,
      title={Walk Like Dogs: Learning Steerable Imitation Controllers for Legged Robots from Unlabeled Motion Data}, 
      author={Dongho Kang and Jin Cheng and Fatemeh Zargarbashi and Taerim Yoon and Sungjoon Choi and Stelian Coros},
      year={2026},
      eprint={2507.00677},
      archivePrefix={arXiv},
      primaryClass={cs.RO},
      url={https://arxiv.org/abs/2507.00677}, 
}
{% endhighlight %}

-----

# Acknowledgment

This work has received funding from the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (grant agreement No. 866480.)
