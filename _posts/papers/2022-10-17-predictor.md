---
layout: paper
categories: papers
permalink: papers/conformal_prediction
id: conformal_prediction
title: "Conformalization of Sparse Generalized Linear Models"
venue: International Conference of Machine Learning 2023
venue-shorthand: ICML
year: 2023
url: /papers/general_cp
pdf: https://proceedings.mlr.press/v202/guha23b.html
feature-title: Conformal Prediction
feature-description: "Conformalization of Sparse Generalized Linear Models"
image: /images/featured/cpranks_robust_friedman2.png
feature-order: 1
featured: false
selected: false
type: conference
authors:
    - Etash Guha
    - Eugene Ndiaye
    - Xiaoming Huo
---
Given a sequence of observable variables $(x_1, y_1), \ldots, (x_n, y_n)$, the conformal prediction method estimates a confidence set for $y_{n+1}$ given $x_{n+1}$ that is valid for any finite sample size by merely assuming that the distribution is permutation invariant. Although attractive, computing such a set turns out to be infeasible in most regression problems. Indeed, in these cases, the unknown variable $y_{n+1}$ can take an infinite number of possible values, and generating conformal sets requires retraining a predictive model for each of them. In this paper, we focus on a sparse model where only a subset of variables is used for prediction, and we leverage numerical continuation techniques to efficiently approximate the solution path. The key property we exploit is that the set of selected variables is invariant under a small perturbation of the input data. Therefore, it is sufficient to enumerate and refit the model only at the change points of the set of active features and smoothly interpolate the rest of the solution via a predictor-corrector mechanism. We show how our path-following algorithm accurately approximates conformal prediction sets and illustrate its performance using synthetic and real data examples.