---
layout: paper
categories: papers
permalink: papers/invlinban
id: invlinban
title: "Inverse Reinforcement Learning for Phased Elimination of Linear Stochastic Bandits"
venue: pre-print 2022
venue-shorthand: pre-print
year: 2022
url: /papers/invlinban
pdf: /papers/OPT2022temp.pdf
feature-title: Inverse Reinforcement Learning
feature-description: "Inverse Reinforcement Learning"
image: /images/featured/linear_bandit.png
feature-order: 3
featured: true
selected: true
type: conference
authors:
    - Etash Guha
    - Jim James
    - Krishna Acharya
    - Ashwin Pananjady
    - Vidya Muthukumar
---
Given a sequence of observable variables $(x_1, y_1), \ldots, (x_n, y_n)$, the conformal prediction method estimates a confidence set for $y_{n+1}$ given $x_{n+1}$ that is valid for any finite sample size by merely assuming that the distribution is permutation invariant. Although attractive, computing such a set turns out to be infeasible in most regression problems. Indeed, in these cases, the unknown variable $y_{n+1}$ can take an infinite number of possible values, and generating conformal sets requires retraining a predictive model for each of them. In this paper, we focus on a sparse model where only a subset of variables is used for prediction, and we leverage numerical continuation techniques to efficiently approximate the solution path. The key property we exploit is that the set of selected variables is invariant under a small perturbation of the input data. Therefore, it is sufficient to enumerate and refit the model only at the change points of the set of active features and smoothly interpolate the rest of the solution via a predictor-corrector mechanism. We show how our path-following algorithm accurately approximates conformal prediction sets and illustrate its performance using synthetic and real data examples.