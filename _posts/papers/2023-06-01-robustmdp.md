---
layout: paper
categories: papers
permalink: papers/robustmdp
id: robustmdp
title: "Solving Robust MDPs through No-Regret Dynamics"
venue: Under Review
year: 2023
url: /papers/robustmdp
pdf: https://arxiv.org/abs/2305.19035
feature-title: Robust MDPs
feature-description: "Solving Robust MDPs through No-Regret Dynamics"
image: /images/featured/rl.png
feature-order: 2
featured: true
selected: true
type: conference
authors:
    - Etash Guha
    - Jason D. Lee
---
 Reinforcement Learning is a powerful framework for training agents to navigate different situations, but it is susceptible to changes in environmental dynamics. However, solving Markov Decision Processes that are robust to changes is difficult due to nonconvexity and size of action or state spaces. While most works have analyzed this problem by taking different assumptions on the problem, a general and efficient theoretical analysis is still missing. However, we generate a simple framework for improving robustness by solving a minimax iterative optimization problem where a policy player and an environmental dynamics player are playing against each other. Leveraging recent results in online nonconvex learning and techniques from improving policy gradient methods, we yield an algorithm that maximizes the robustness of the Value Function on the order of $\mathcal{O}\left(\frac{1}{T^{\frac{1}{2}}}\right)$ where $T$ is the number of iterations of the algorithm. 