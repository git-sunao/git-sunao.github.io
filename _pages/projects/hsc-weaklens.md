---
title: HSC cosmology
permalink: /projects/hsc-weaklens
layout: archive
mathjax: true
author_profile: true
---

![hsc-weaklens](/assets/images/hscweaklensy1.jpg)

Using the Subaru HSC Y1 data, we performed so-called 2$$\times$$2pt analysis, i.e. a joint analysis of galaxy-galaxy lensing and galaxy clustering.
We used the HSC Y1 shape catalog for weak lens galaxy, and SDSS spectroscopic galaxy catalog for lens galaxy.
Galaxies are the biased tracer of the underlying matter density field, and thus we need to use the galaxy bias model for the robust estimation of cosmological parameters.
For the HSC Y1 data, we develop two galaxy bias models: the minimal bias model which is inspired by the cosmological perturbation theory and valid on sufficiently large scale, and the halo-based model which can predict the nonlinear physics down to relatively small scales than the minimal bias model.
In order to validate the use of galaxy models above in the cosmological parameter inference from Subaru HSC 2$$\times$$2pt analysis, we performed the _cosmology challenge_, where we analyze the mock data and test the model by checking the input cosmological parameters can be recovered by the analysis (see [Sugiyama et al.](https://arxiv.org/abs/2008.06873) for minimal bias model validation and [Miyatake et al.](https://arxiv.org/abs/2101.00113) for halo-based model validation).
Based on these studies, we find the scale where these models can be applied to robustly infer the true cosmological parameters.

We applied these models (minimal bias model and halo-based model) to the HSC Y1 real data in [Sugiyama et al.](https://arxiv.org/abs/2111.10966) and [Miyatake et al.](https://arxiv.org/abs/2111.02419).
To avoid the confirmation bias of the analyst, we performed the blind analysis, where we analyzed three blind catalogs. We also blinded the value of cosmological parameter values in the blind analysis to prevent ourselves to compare the result of HSC to thost from external experiments, e.g. Planck.
During the blind analysis we performed various kind of systematics tests, and unblinded our result after we confirmed that our analysis are bias free.
We find $$S_8=0.795^{+0.049}_{−0.042}$$, which is consistent with Planck 2018, indicating no $$S_8$$ tension.