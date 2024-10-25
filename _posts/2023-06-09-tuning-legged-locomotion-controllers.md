---
title: "Tuning Legged Locomotion Controllers via Safe Bayesian Optimization"
description: 7th Annual Conference on Robot Learning (CoRL 2023)
layout: distill
published: true
date: 2023-06-08 13:58:00
img: /assets/img/widmer2023tuning/widmer2023tuning.png
permalink: /tuning-legged-locomotion-controllers/
tags: [robotics, conference]
categories: research
authors:
  - name: Daniel Widmer<sup>*</sup><d-footnote>* The first two authors contributed equally.</d-footnote>
    affiliations:
      name: D-MAVT<d-footnote>Dept. of Mechanical and Process Engineering</d-footnote>, ETH Zurich
  - name: Dongho Kang<sup>*</sup>
    url: "https://donghok.me/"
    affiliations:
      name: CRL<d-footnote>Computational Robotics Lab.</d-footnote>, ETH Zurich
  - name: Bhavya Sukhija
    url: "https://sukhijab.github.io/"
    affiliations:
      name: CRL & LAS<d-footnote>Learning & Adaptive Systems Group</d-footnote>, ETH Zurich
  - name: Jonas Hübotter
    affiliations:
      name: LAS, ETH Zurich
  - name: Andreas Krause
    url: "https://las.inf.ethz.ch/krausea"
    affiliations:
      name: LAS, ETH Zurich
  - name: Stelian Coros
    url: "http://crl.ethz.ch/people/coros/index.html"
    affiliations:
      name: CRL, ETH Zurich
bibliography:
---

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
      <img class="img-fluid" src="{{ '/assets/img/widmer2023tuning/widmer2023tuning.png' | relative_url }}" alt="" title="teaser"/>
  </div>
</div>

<br> 

# Abstract

This paper presents a data-driven strategy to streamline the deployment of model-based controllers in legged robotic hardware platforms. 
Our approach leverages a model-free safe learning algorithm to automate the tuning of control gains, addressing the mismatch between the simplified model used in the control formulation and the real system.
This method substantially mitigates the risk of hazardous interactions with the robot by sample-efficiently optimizing parameters within a probably safe region.
Additionally, we extend the applicability of our approach to incorporate the different gait parameters as contexts, leading to a safe, sample-efficient exploration algorithm capable of tuning a motion controller for diverse gait patterns.
We validate our method through simulation and hardware experiments, where we demonstrate that the algorithm obtains superior performance on tuning a model-based motion controller for multiple gaits safely.

**Paper: [[PMLR](https://proceedings.mlr.press/v229/widmer23a.html)]** &emsp; **Open access: [[ArXiv](https://arxiv.org/abs/2306.07092)]** &emsp; **Code: [[GitHub](https://github.com/lasgroup/gosafeopt)]**

-----

# Full Supplementary Video

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/zVm7IkYofbg" allowfullscreen></iframe>
</div>  

-----

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

This project has received funding from the Swiss National Science Foundation under NCCR Automation, grant agreement 51NF40 180545, the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme, grant agreement No. 866480, and the Microsoft Swiss Joint Research Center.