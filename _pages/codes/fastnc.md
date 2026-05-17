---
title: fastnc
permalink: /codes/fastnc
layout: archive
mathjax: true
author_profile: true
classes: justify-text
---

Code: [fastnc](https://github.com/git-sunao/fastnc)

To compute 3PCF from the underlying matter bispectrum, we need to perform a multidimensional Fourier transformation, which is difficult especially because cosmic shear 3PCF include the phase factor that makes integrand oscilates a lot. In [Sugiyama+2024](https://arxiv.org/abs/2407.01798), we developed a novel algorithm that compute the shear 3PCF from bispectrum, using the multipole decomposition of the 3PCF and bispectrum into multipoles. The multipoles in real and Fourier space are related to each other through a 2D Hankel transform, which can be performed quite efficiently using 2D FFTLog. This software implement this idea, and enabled the cosmology inference through a joint analysis of 2+3PCF. See [Sugiyama+2025](https://arxiv.org/abs/2508.14018) and [Gomes, Sugiyama+2025](https://arxiv.org/abs/2508.14019) for DES and HSC application respectively.