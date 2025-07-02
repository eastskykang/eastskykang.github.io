---
title: "Learning Steerable Imitation Controllers From Unstructured Animal Motions"
description: ArXiv
layout: distill
published: true
date: 2025-07-02 22:39:00
img: /assets/img/kang2025learning/teaser.jpg
permalink: /learning-steerable-imitation-controllers/
tags: [robotics]
categories: research
authors:
  - name: Dongho Kang
    url: "https://donghok.me/"
    affiliations:
      name: CRL<d-footnote>Computational Robotics Lab.</d-footnote>, ETH Zurich
  - name: Jin Cheng
    url: "https://jin-cheng.me/"
    affiliations:
      name: CRL, ETH Zurich
  - name: Fatemeh Zargarbashi
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

This paper presents a control framework for legged robots that leverages unstructured real-world animal motion data to generate animal-like and user-steerable behaviors. Our framework learns to follow velocity commands while reproducing the diverse gait patterns in the original dataset. To begin with, animal motion data is transformed into a robot-compatible database using constrained inverse kinematics and model predictive control, bridging the morphological and physical gap between the animal and the robot. Subsequently, a variational autoencoder-based motion synthesis module captures the diverse locomotion patterns in the motion database and generates smooth transitions between them in response to velocity commands. The resulting kinematic motions serve as references for a reinforcement learning-based feedback controller deployed on physical robots. We show that this approach enables a quadruped robot to adaptively switch gaits and accurately track user velocity commands while maintaining the stylistic coherence of the motion data. Additionally, we provide component-wise evaluations to analyze the system's behavior in depth and demonstrate the efficacy of our method for more accurate and reliable motion imitation.

**Open access: [[ArXiv](https://arxiv.org/abs/2507.00677)]**

-----

# Full Supplementary Video

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/DukyUGNYf5A" allowfullscreen></iframe>
</div>  

<!-- -----

# Bibtex

{% highlight txt %}
@InProceedings{pmlr-v229-widmer23a,
  title = {Tuning Legged Locomotion Controllers via Safe Bayesian Optimization},
  author = {Widmer, Daniel and Kang, Dongho and Sukhija, Bhavya and H\"{u}botter, Jonas and Krause, Andreas and Coros, Stelian},
  booktitle = {Proceedings of The 7th Conference on Robot Learning},
  pages = {2444--2464},
  year = {2023},
  editor = {Tan, Jie and Toussaint, Marc and Darvish, Kourosh},
  volume = {229},
  series = {Proceedings of Machine Learning Research},
  month = {06--09 Nov},
  publisher = {PMLR}
}
{% endhighlight %}

-----

# Acknowledgment

We would like to thank Lenart Treven and Flavio De Vincenti for their feedback on this work. 

This project has received funding from the Swiss National Science Foundation under NCCR Automation, grant agreement 51NF40 180545, the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme, grant agreement No. 866480, and the Microsoft Swiss Joint Research Center. -->