---
title: "RL + Model-based Control: Using On-demand Optimal Control to Learn Versatile Legged Locomotion"
description: IEEE Robotics and Automation Letters (RA-L)
layout: distill
published: true
date: 2023-05-27 16:10:33
img: /assets/img/kang2023rl/kang2023rl.png
permalink: /rl-plus-model-based-control/
tags: [robotics, journal]
categories: publication
authors:
  - name: Dongho Kang
    url: "https://donghok.me/"
    affiliations:
      name: CRL<d-footnote>Computational Robotics Lab.</d-footnote>, ETH Zurich
  - name: Jin Cheng
    affiliations:
      name: CRL, ETH Zurich
  - name: Miguel Zamora
    affiliations:
      name: CRL, ETH Zurich
  - name: Fatemeh Zargarbashi
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
      <img class="img-fluid" src="{{ '/assets/img/kang2023rl/kang2023rl.png' | relative_url }}" alt="" title="teaser"/>
  </div>
</div>

<br>

# Abstract

This letter presents a control framework that combines model-based optimal control and reinforcement learning (RL) to achieve versatile and robust legged locomotion. 
Our approach enhances the RL training process by incorporating on-demand reference motions generated through finite-horizon optimal control, covering a broad range of velocities and gaits.
These reference motions serve as targets for the RL policy to imitate, leading to the development of robust control policies that can be learned with reliability. 
Furthermore, by utilizing realistic simulation data that captures whole-body dynamics, RL effectively overcomes the inherent limitations in reference motions imposed by modeling simplifications. 
We validate the robustness and controllability of the RL training process within our framework through a series of experiments. 
In these experiments, our method showcases its capability to generalize reference motions and effectively handle more complex locomotion tasks that may pose challenges for the simplified model, thanks to RL’s flexibility. 
Additionally, our framework effortlessly supports the training of control policies for robots with diverse dimensions, eliminating the necessity for robot-specific adjustments in the reward function and hyperparameters.

**Paper: [<a href="https://ieeexplore.ieee.org/document/10225268">IEEE Xplore</a>]** &emsp; **Open access: [<a href="https://arxiv.org/abs/2305.17842">ArXiv</a>]**

-----

# Supplementary Video

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/HXwLXdOf79c" allowfullscreen></iframe>
</div>  

-----

# Presentation

We are pleased to announce that our paper has been selected for presentation at <a href="https://2024.ieee-icra.org/">ICRA 2024 in Yokohama, Japan</a>. 
Please join us for our oral presentation in the "Legged Robot III" session on May 14th from 16:30 to 18:00, and for our poster presentation session earlier that day from 10:30 to 12:00. 
We are excited to share our work with you and look forward to seeing you there.

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/U4tCgsEFJmM" allowfullscreen></iframe>
</div>  

-----

# Demos

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/PCT5f6xsASk" allowfullscreen></iframe>
</div>

<br>

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/30CmkKIJ2fQ" allowfullscreen></iframe>
</div>  

<br>

<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/-tUdeYsNvSQ" allowfullscreen></iframe>
</div>  

-----

# Bibtex

{% highlight txt %}
@article{kang2023rl,
  author={Kang, Dongho and Cheng, Jin and Zamora, Miguel and Zargarbashi, Fatemeh and Coros, Stelian},
  journal={IEEE Robotics and Automation Letters}, 
  title={RL + Model-Based Control: Using On-Demand Optimal Control to Learn Versatile Legged Locomotion}, 
  year={2023},
  volume={8},
  number={10},
  pages={6619-6626},
  doi={10.1109/LRA.2023.3307008}
}
{% endhighlight %}

-----

# Acknowledgment

This work has received funding from the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (grant agreement No. 866480.)

We express our gratitude to Zijun Hui for his assistance with the robot experiments.
  