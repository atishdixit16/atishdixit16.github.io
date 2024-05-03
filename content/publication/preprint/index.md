---
title: "A Multilevel Reinforcement Learning Framework for PDE-based Control"
authors:
- admin
date: "2019-04-07T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2022-10-28T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: ""

abstract: Reinforcement learning (RL) is a promising method to solve control problems. However, model-free RL algorithms are sample inefficient and require thousands if not millions of samples to learn optimal control policies. A major source of computational cost in RL corresponds to the transition function, which is dictated by the model dynamics. This is especially problematic when model dynamics is represented with coupled PDEs. In such cases, the transition function often involves solving a large-scale discretization of the said PDEs. We propose a multilevel RL framework in order to ease this cost by exploiting sublevel models that correspond to coarser scale discretization (i.e. multilevel models). This is done by formulating an approximate multilevel Monte Carlo estimate of the objective function of the policy and / or value network instead of Monte Carlo estimates, as done in the classical framework. As a demonstration of this framework, we present a multilevel version of the proximal policy optimization (PPO) algorithm. Here, the level refers to the grid fidelity of the chosen simulation-based environment. We provide two examples of simulation-based environments that employ stochastic PDEs that are solved using finite-volume discretization. For the case studies presented, we observed substantial computational savings using multilevel PPO compared to its classical counterpart.

# Summary. An optional shortened abstract.
summary: We introduce a multilevel reinforcement learning framework to reduce computational costs associated with model dynamics represented by coupled PDEs, offering significant savings compared to traditional methods. By leveraging sublevel models and an approximate multilevel Monte Carlo estimate, our approach demonstrates improved efficiency in solving control problems with stochastic PDE-based environments.

tags:
- Source Themes
featured: false

links:
- name: Custom Link
  url: http://example.org
url_pdf: https://arxiv.org/pdf/2210.08400
url_code: 'https://github.com/atishdixit16/stable-baselines3/tree/d60610b5709ea7910bdad6b52b4347df6bded6ec'
url_dataset: '#'
url_poster: '#'
url_project: ''
url_slides: ''
url_source: '#'
url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---

{{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).
