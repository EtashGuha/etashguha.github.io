---
layout: paper
categories: papers
permalink: papers/openthoughts
id: openthoughts
title: "OpenThoughts: Data Recipes for Reasoning Models"
venue: pre-print
venue-shorthand: pre-print
year: 2025
url: /papers/openthoughts
pdf: https://arxiv.org/abs/2506.04178
feature-title: OpenThoughts
feature-description: OpenThoughts
image: /images/featured/open_thoughts_full2.png
feature-order: 1
featured: true
selected: true
type: conference
authors:
    - Etash Guha*
    - Ryan Marten*
    - Sedrick Keh*
    - Negin Raoof*
    - Georgios Smyris* 
    - (many not shown)
    - Alex Dimakis
    - Ludwig Schmidt
---
Reasoning models have made rapid progress on many benchmarks involving math, code, and science. Yet, there are still many open questions about the best training recipes for reasoning since state-of-the-art models often rely on proprietary datasets with little to no public information available. To address this, the goal of the OpenThoughts project is to create open-source datasets for training reasoning models. After initial explorations, our OpenThoughts2-1M dataset led to OpenThinker2-32B, the first model trained on public reasoning data to match DeepSeek-R1-Distill-32B on standard reasoning benchmarks such as AIME and LiveCodeBench. We then improve our dataset further by systematically investigating each step of our data generation pipeline with 1,000+ controlled experiments, which led to OpenThoughts3. Scaling the pipeline to 1.2M examples and using QwQ-32B as teacher yields our OpenThoughts3-7B model, which achieves state-of-the-art results: 53% on AIME 2025, 51% on LiveCodeBench 06/24-01/25, and 54% on GPQA Diamond - improvements of 15.3, 17.2, and 20.5 percentage points compared to the DeepSeek-R1-Distill-Qwen-7B. All of our datasets and models are available on https://www.openthoughts.ai/.