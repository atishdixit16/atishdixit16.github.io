---
title: Reproducibility in Deep Reinforcement Learning Literature
date: '2023-11-04'
summary: A post on importance of reproducibility in reinforcement learning literature using example of my paper on multilevel PPO
---

It's surprising to see how many research papers in reinforcement learning (RL) lack reproducibility in their implementation. Alarmingly, this issue persists even in high-ranking machine learning journals, which are often essential for securing positions in leading AI companies. This problem seems to stem from the immense pressure in academia to publish frequently, as it is a key factor for career advancement. However, this practice has significant negative consequences:

1. **Reduced Reliability**: It undermines the credibility of prestigious journals.
2. **Research Confusion**: It leads to confusion among researchers who rely on these papers as a foundation for their work.
3. **Misguided Progress**: It can steer the field in a false direction, hindering genuine advancements.

Given these concerns, I want to emphasize the critical importance of reproducibility in research. To illustrate, I'll share an example from my recent paper, where I introduced an algorithm called Multilevel PPO.
    
![png](example.png)
    

```python
print("Welcome to Academic!")
```

    Welcome to Academic!

## Organize your notebooks

Place the notebooks that you would like to publish in a `notebooks` folder at the root of your website.

## Import the notebooks into your site

```bash
pipx install academic
academic import 'notebooks/**.ipynb' content/post/ --verbose
```

The notebooks will be published to the folder you specify above. In this case, they will be published to your `content/post/` folder.
