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

Reinforcement learning (RL) has long been hailed as the silver bullet for solving complex control problems, promising autonomous systems that can learn and adapt. Yet, despite its potential, RL has often been criticized for its insatiable appetite for data. Traditional model-free RL algorithms demand thousands, if not millions, of samples to converge to optimal control policies, rendering them inefficient and computationally expensive.

One of the primary culprits behind this voracious need for data is the transition function, which dictates how the system evolves from one state to another. In scenarios where model dynamics are described by coupled Partial Differential Equations (PDEs), the transition function becomes especially cumbersome. Here, solving a large-scale discretization of these PDEs adds significant computational overhead, impeding the scalability and practicality of RL algorithms.

But fear not, for there is hope on the horizon in the form of a revolutionary approach – the multilevel RL framework. Drawing inspiration from Giles (2015), this innovative paradigm leverages sublevel models corresponding to coarser scale discretizations, known as multilevel models. Instead of trudging through the intricacies of high-fidelity simulations for every decision, multilevel RL takes a more strategic approach.

How does it work? By formulating an approximate multilevel Monte Carlo estimate of the objective function of the policy and/or value network, we sidestep the need for exhaustive Monte Carlo estimates. This allows us to operate on a spectrum of grid fidelities in our simulation-based environment, adapting our computational resources to match the complexity of the task at hand.

To demonstrate the prowess of this game-changing framework, we introduce a multilevel version of the proximal policy optimization (PPO) algorithm. In our experiments, the "level" refers to the grid fidelity of the chosen simulation-based environment. We delve into two case studies featuring stochastic PDEs, solved using finite-volume discretization, showcasing the tangible benefits of multilevel PPO over its classical counterpart.

The results? Astounding computational savings that pave the way for RL to tackle larger and more intricate control problems with ease. With multilevel frameworks at our disposal, the era of sample inefficiency in RL may soon be a relic of the past. As we continue to push the boundaries of what's possible in autonomous systems, multilevel RL stands as a beacon of innovation, offering a tantalizing glimpse into the future of intelligent control.

