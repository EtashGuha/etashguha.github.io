---
layout: paper
categories: papers
permalink: papers/plasticity
id: plasticity
title: "Learning with Plasticity Rules: Generalization and Robustness"
venue: pre-print 2021
venue-shorthand: pre-print
year: 2022
url: /papers/plasticity
pdf: /papers/learning_with_plasticity_rules.pdf
feature-title: Hebbian Plasticity
feature-description: "Learning with Plasticity Rules: Generalization and Robustness"
image: /images/featured/hebbian_pic.png
feature-order: 3
featured: true
selected: true
type: conference
---

Brains learn robustly, and generalize effortlessly between different learning
tasks; in contrast, robustness and generalization across tasks are well known
weaknesses of artificial neural nets (ANNs). How can we use our accelerating
understanding of the brain to improve these and other aspects of ANNs?
Here we hypothesize that (a) Brains employ synaptic plasticity rules that
serve as proxies for Gradient Descent (GD); (b) These rules themselves
can be learned by GD on the rule parameters; and (c) This process may
be a missing ingredient for the development of ANNs that generalize well
and are robust to adversarial perturbations. We provide both empirical
and theoretical evidence for this hypothesis. In our experiments, plasticity
rules for the synaptic weights of recurrent neural nets (RNNs) are learned
through GD and are found to perform reasonably well (with no backpropagation). We find that plasticity rules learned by this process generalize from
one type of data/classifier to others (e.g., rules learned on synthetic data
work well on MNIST/Fashion MNIST) and converge with fewer updates.
Moreover, the classifiers learned using plasticity rules exhibit surprising
levels of tolerance to adversarial perturbations. In the special case of the
last layer of a classification network, we show analytically that GD on the
plasticity rule recovers (and improves upon) the perceptron algorithm and
the multiplicative weights method. Finally, we argue that applying GD to
learning rules is biologically plausible, in the sense that it can be learned
over evolutionary time: we describe a genetic setting where natural selection
of a numerical parameter over a sequence of generations provably simulates
a simple variant of GD.