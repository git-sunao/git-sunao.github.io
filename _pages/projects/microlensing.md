---
title: Microlensing
permalink: /projects/microlensing
layout: archive
mathjax: true
author_profile: true
classes: justify-text
---

## Papers
### Microlensing observation for PBH search
[Sugiyama+2026](https://arxiv.org/abs/2602.05840) analyzed the latest data of Subaru Hyper Suprime-Cam (HSC) survey to search for microlensing events caused by primordial black holes (PBHs) in the Milky Way halo. This is an extended analysis of our previous work [Niikura+2019](https://arxiv.org/abs/1701.02151) using the 2014 one-night HSC data. We extended our microlensing temlate to include the finite source size effect and the wave optics effect, which are important for constraining small PBHs.

### Finite-source size effect
Finite-source size effect (or extended source effect) is an important effect for microlensing. Modeling this effect requires an convolution of the point-source magnification with the surface brightness profile of the source star. We developed a new method to perform this convolution efficiently, which is described in [Sugiyama2022](https://arxiv.org/abs/2203.06637). This method is based on the idea of the fast Fourier transform (FFT) and can be applied to various surface brightness profiles, including limb-darkened profiles. We also provide a public code for this method, which is available at [fastlens](https://github.com/git-sunao/fft-extended-source).


### Exploring Primordial Black Holes from the Multiverse with Optical Telescopes
In [Kusenko+2020](https://arxiv.org/abs/2001.09160), we studied a multiverse-motivated scenario in which primordial black holes form from false-vacuum bubble nucleation during inflation. This mechanism naturally produces a broad PBH mass spectrum, spanning masses relevant to dark matter, the Subaru/HSC microlensing candidate event, LIGO black holes, and possible seeds of supermassive black holes. We showed that optical microlensing surveys, especially high-cadence observations with Subaru/HSC, can provide a direct observational test of whether this PBH population makes up the dark matter.

### Wave optics effect
In [Sugiyama+2020](https://arxiv.org/abs/1905.06066) We studied wave-optics effects in optical microlensing by primordial black holes, focusing on the low-mass regime where the Schwarzschild radius of the lens becomes comparable to the wavelength of observed light. In this regime, the usual geometric-optics approximation is modified, and the microlensing light curve can acquire characteristic interference features. We quantified how these effects change PBH microlensing signals and examined their impact on constraints from Subaru/HSC observations of M31. We found that, for the relevant PBH mass range around $$10^{-11} - 10^{-10}M_\odot$$, finite-source-size effects are more important than wave-optics corrections for current M31 microlensing constraints.

### Niikura+2019
![microlensing](/assets/images/microlensing.jpg)
In [Niikura+2019](https://arxiv.org/abs/1701.02151), we conducted a search for microlensing events in the Subaru Hyper Suprime-Cam (HSC) survey of the Andromeda galaxy (M31) to constrain the abundance of primordial black holes (PBHs) in the mass range $$10^{-11} - 10^{-6}M_\odot$$. We analyzed data from a single night of HSC observations toward M31.


## Related press releases
- [this press release](https://www.ipmu.jp/en/20201224-PBH-multiverse) for vaccum bubble model.
- [this press release](https://www.ipmu.jp/en/20190402-PrimordialBlackHole) for PBH observation.


## Related press codes
- [fastlens](/codes/fastlens)