---
layout: archive
title: Codes
permalink: /codes/
author_profile: true
mathjax: true
---

### [fft-extended-source](https://github.com/git-sunao/fft-extended-source)

FFT based evaluation of finite source effect on microlensing. See and cite [Sugiyama](https://arxiv.org/abs/2203.06637).
This method reduces the two-dimensional integration to one-dimensional fft on logarithmic space, which can be efficiently evaluated.
The target quantity to be evaluated is

$$
\tilde{A}_{\rm ext}(u; \rho) = \int{\rm d}\vec{x} A_{\rm p}(\vec{x})s(\vec{x}+\vec{u};\rho).
$$

where $$s(u;\rho)$$ is the source flux profile as a function of distance from source center, $$u$$.

### [dark_emulator_public](https://github.com/DarkQuestCosmology/dark_emulator_public)

Dark Emulator is an emulator of cosmological dark matter halo statistics.
Dark Emulator is a part of the [dark quest project](https://darkquestcosmology.github.io/).
This is based on [Nishimichi et al](https://arxiv.org/abs/1811.09504).
This package includes the linear power spectrum (of CAMB) emulator in itself.
