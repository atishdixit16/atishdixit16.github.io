---
title: Multilevel Deep Reinforcement Learning Framework
summary: A statistical framework to reduce computational complexity of RL applications in computational physics based environments
tags:
  - Deep Learning
date: '2016-04-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
  - icon: linkedin
    icon_pack: fab
    name: Follow
    url: https://www.linkedin.com/in/atish-dixit-14461518/
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ''
---

Reinforcement learning (RL) has long been recognized as a promising approach for tackling complex control problems. However, its model-free algorithms often demand a huge amount of data to learn optimal control policies, making them inefficient and computationally intensive.

A significant contributor to this computational burden is the transition function, particularly in cases where model dynamics are described by coupled Partial Differential Equations (PDEs). Here, solving large-scale discretizations of these PDEs adds considerable overhead to RL algorithms, hindering their scalability.

Enter the multilevel RL framework. Inspired by Giles (2015), this approach utilizes sublevel models corresponding to coarser scale discretizations, termed multilevel models. By approximating the objective function of the policy and/or value network using a multilevel Monte Carlo estimate, we can bypass the need for exhaustive Monte Carlo estimates and adapt computational resources to the task's complexity.

To demonstrate this framework's effectiveness, I've implemented a multilevel version of the proximal policy optimization (PPO) algorithm. In our experiments, the "level" corresponds to the grid fidelity of the simulation-based environment. We've explored two case studies featuring stochastic PDEs solved using finite-volume discretization, highlighting the computational savings achieved with multilevel PPO compared to its classical counterpart.

The results are promising, showing significant computational efficiencies that could pave the way for RL to tackle larger and more complex control problems. With multilevel frameworks, we're poised to overcome the sample inefficiency challenges that have plagued RL, offering a practical pathway towards more efficient and scalable intelligent control systems.
