---
title: 3PCF cosmology
permalink: /projects/weaklens-23pcf
layout: archive
mathjax: true
author_profile: true
classes: justify-text
---

## Papers
### HSC Year 3 cosmic shear 2+3PCF cosmology
![cosmology23pcf](/assets/images/cosmo23pcf.png)
In [Sugiyama+2025](https://arxiv.org/abs/2508.14019), we performed a joint cosmological analysis of the cosmic shear two-point and three-point correlation functions using Subaru Hyper Suprime-Cam Year 3 data. This work extends HSC weak-lensing cosmology beyond standard two-point statistics by extracting non-Gaussian information from real survey data. We demonstrated the feasibility of applying three-point cosmic shear statistics to HSC data and provided a practical step toward higher-order weak-lensing analyses for current and future galaxy surveys.

### DES Year 3 cosmic shear 2+3PCF cosmology

In [Gomes, Sugiyama, Jain+2025](https://arxiv.org/abs/2508.14018), we applied a second- and third-order weak-lensing analysis framework to Dark Energy Survey Year 3 data. We measured tomographic higher-order shear information using the third-order aperture mass statistic and combined it with standard two-point cosmic shear statistics. This work showed that higher-order weak-lensing statistics can be applied to current survey data at cosmological-analysis level and can improve constraints on parameters such as $$(\Omega_{\rm m} and S_8$$.

### Intrinsic-alignment modeling for higher-order weak lensing

In [Gomes, Miller, Sugiyama+2025](https://arxiv.org/abs/2601.09133), we developed a model for intrinsic-alignment contamination in the cosmic shear three-point correlation function and aperture-mass skewness using the tidal alignment and tidal torquing framework. We connected TATT-based intrinsic-alignment bispectra to practical predictions for higher-order weak-lensing statistics and compared NLA, TATT, and extended TATT models. We showed that intrinsic alignments can significantly affect specific three-point configurations and that joint two- and three-point analyses can help break degeneracies between cosmology and intrinsic-alignment parameters.

### Methodology for DES cosmic shear 2+3PCF cosmology

In [Gomes, Sugiyama, Jain+2025](https://arxiv.org/abs/2503.03964), we developed and validated a cosmological inference pipeline for combining second- and third-order cosmic shear statistics. The pipeline includes fast theoretical predictions for three-point shear correlations using `fastnc`, integration with the CosmoSIS framework, covariance estimation from simulations, and likelihood validation with mock analyses. This work established the modeling, measurement, and inference framework needed for robust cosmological constraints from higher-order weak-lensing statistics, serving as the foundation for the subsequent DES Year 3 data analysis.

### fastnc: Fast modeling of the shear three-point correlation function
In [Sugiyama, Gomes, Jarvis+2024](https://arxiv.org/abs/2407.01798), we developed a fast and accurate method to compute theoretical predictions for the weak-lensing shear three-point correlation function. The method uses a multipole expansion of the matter bispectrum, avoiding expensive direct numerical integration and making three-point shear modeling practical for cosmological analyses. We showed that the method can compute the shear 3PCF with percent-level accuracy on short timescales, including tomographic source-bin configurations and bin-averaging effects. This work provides the theoretical modeling foundation for applying higher-order weak-lensing statistics to real survey data from HSC, DES, and future galaxy surveys.

## Related press codes
- [fastnc](/codes/fastnc)
- [p-MOPED](/codes/pmoped)
- [interactive3pcf](/codes/interactive3pcf)