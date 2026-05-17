---
title: fastlens
permalink: /codes/fastlens
layout: archive
mathjax: true
author_profile: true
classes: justify-text
---

Code: [fastlens](https://github.com/git-sunao/fft-extended-source)

`fastlens` is an FFT based evaluation of finite source effect on microlensing. See and cite [Sugiyama](https://arxiv.org/abs/2203.06637).
This method reduces the two-dimensional integration to one-dimensional fft on logarithmic space, which can be efficiently evaluated.
The target quantity to be evaluated is

$$
A_{\rm ext}(u; \rho) = \int{\rm d}\vec{x} A_{\rm p}(\vec{x})s(\vec{x}+\vec{u};\rho).
$$

where $$s(u;\rho)$$ is the source flux profile as a function of distance from source center, $$u$$.

`fastlens` is installable from both pip and conda:
```
pip install fastlens
```
or 
```
conda install -c ssunao fastlens
```