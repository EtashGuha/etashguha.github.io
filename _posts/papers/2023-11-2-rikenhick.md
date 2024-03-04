---
layout: paper
categories: papers
permalink: papers/cl
id: cl
title: "On the Diminishing Returns of Width for Continual Learning"
venue: ICLR 2024 Workshop on Bridging the Gap Between Practice and Theory in Deep Learning
url: /papers/cl
pdf: /papers/Go_Sparse_and_Wide_to_Forget_Less.pdf
feature-title: Continual Learning
feature-description: "Continual Learning"
image: /images/featured/cpranks_robust_friedman2.png
feature-order: 1
featured: false
selected: true
type: conference
authors:
    - Etash Guha
    - Vihan Lakshman
---
Conformal prediction (CP) for regression can be challenging, especially when the output distribution is heteroscedastic, multimodal, or skewed. Some of the issues can be addressed by estimating a distribution over the output, but in reality, such approaches can be sensitive to estimation error and yield unstable intervals.~Here, we circumvent the challenges by converting regression to a classification problem and then use CP for classification to obtain CP sets for regression.~To preserve the ordering of the continuous-output space, we design a new loss function and present necessary modifications to the CP classification techniques.~Empirical results on many benchmarks shows that this simple approach gives surprisingly good results on many practical problems.