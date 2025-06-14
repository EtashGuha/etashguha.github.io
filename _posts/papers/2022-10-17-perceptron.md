---
layout: paper
categories: papers
permalink: papers/perceptron
id: perceptron
title: "On Accelerated Perceptrons and Beyond"
venue: International Conference of Learning Representations 2023
venue-shorthand: ICLR
year: 2023
url: https://arxiv.org/abs/2210.09371
pdf: https://arxiv.org/abs/2210.09371
feature-title: Accelerated Perceptrons
feature-description: "On Accelerated Perceptrons and Beyond"
image: /images/featured/perceptron_image.png
feature-order: 3
featured: false
selected: false
type: conference
authors:
    - Guanghui Wang
    - Rafael Hanashiro
    - Etash Guha
    - Jacob Abernethy
---
The classical Perceptron algorithm of Rosenblatt can be used to find a linear threshold function to correctly classify $n$ linearly separable data points, assuming the classes are separated by some margin $\gamma > 0$. A foundational result is that Perceptron converges after  $\Omega(1/\gamma^{2})$ iterations. There have been several recent works that managed to improve this rate by a quadratic factor, to $\Omega(\sqrt{\log n}/\gamma)$, with more sophisticated algorithms. In this paper, we unify these existing results under one framework by showing that they can all be described through the lens of solving min-max problems using modern acceleration techniques, mainly through \emph{optimistic} online learning.  We then show that the proposed framework also lead to improved results for a series of problems beyond the standard Perceptron setting. Specifically, a) For the \emph{margin maximization} problem, we improve the state-of-the-art result from $O(\log t/t^2)$ to $O(1/t^2)$, where $t$ is the number of iterations; b) We provide the first result on identifying the \emph{implicit bias} property of the classical Nesterov's accelerated gradient descent (NAG) algorithm, and show NAG can maximize the margin with an $O(1/t^2)$ rate; c) For the classical \emph{$p$-norm Perceptron} problem, we provide an algorithm with $\Omega(\sqrt{(p-1)\log n}/\gamma)$ convergence rate, while existing algorithms suffer the $\Omega({(p-1)}/\gamma^2)$ convergence rate.