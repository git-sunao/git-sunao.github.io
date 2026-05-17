---
title: Data Compression
permalink: /projects/data-compression
layout: archive
mathjax: true
author_profile: true
classes: justify-text
---

## Papers
# p-MOPED data compression under noisy covariance
![pmoped](/assets/images/concept_powered_moped.png)
In [Sugiyama and Park 2025](https://arxiv.org/abs/2508.14021), we developed powered MOPED, or $$p$$-MOPED, a data-compression method designed for parameter inference when the covariance matrix is estimated from a limited number of simulations. Standard MOPED preserves Fisher information in idealized settings, but it can still propagate noise from a noisy sample covariance into parameter constraints. The $$p$$-MOPED method suppresses this covariance-noise propagation by applying a tunable power-law transformation to the sample correlation matrix, balancing information retention against noise reduction. We tested the method on toy models and on Subaru Hyper Suprime-Cam Year 3 weak-lensing data, showing that $$p$$-MOPED gives more robust compressed likelihood analyses, especially when the number of simulations is limited.


## Codes
- [p-MOPED](/codes/pmoped)