---
layout: page
title: Thesis at APC
permalink: jobs/thesis-apc-2026/
subtitle: Bayesian pipelines for cosmic shear analyses with the Vera Rubin Observatory LSST
---

- 3-year PhD thesis starting with a 3-month internship.
- supervisors: [Cécile Roucelle](mailto:cecile.roucelle@apc.in2p3.fr), [Éric Aubourg](mailto:aubourg@in2p3.fr	)

During the last decade, cosmology has entered a precision era, leading to the prevalence of the standard cosmological model, ΛCDM. Nevertheless, the main ingredient of this model, the so-called dark energy, remains mysterious while dominating the energy budget of the Universe. Its comprehension is therefore one of the main goals in this domain. **Current and upcoming cosmological surveys, including that of the Euclid satellite, launched two years ago, and the ground-based Legacy Survey of Space and Time (LSST) of the Vera Rubin Observatory starting in 2026, are specifically designed to address this objective**. 

These surveys, when combined, will map thousands of square degrees of sky in a multiwavelength manner with sub-arcsec resolution. This will result in the detection of several tens of billions of sources, enabling a wide range of astrophysical investigations and providing unprecedented constraints on the nature of dark energy and dark matter. The scope of the PhD topic, based in the LSST dark energy science collaboration and LSST Informatics and Statistics Science Collaboration context, will aim to bring new developments for the treatment of cosmic shear. More precisely, the PhD topic discussed here (and the preceding internship) will focus on the detection of sources and treatment of so-called unrecognized blends. We will use machine learning approaches that we want to build into Bayesian pipelines. This is the context of our “AstroDeep” ANR funding, and the direction taken by our research team for the past few years. This PhD topic will be funded as well by this grant.  

##Scientific context : 

The gravitational lensing corresponds to the deflection of light from distant sources (background galaxies) due to the bending of space-time by matter along the line of sight, resulting in  distortions and displacements of their image. The statistical study of weak gravitational lensing distortions at large scales provides a “mapping” of the matter (dark or visible) between the observer and source (well, more accurately, the effect we want to study is the one of the small and coherent deformation of background galaxies following the principle described here and which is called cosmic shear). The measurement of cosmic shear (and its combination with other probes) gives a window on the properties and the evolution of cosmic structures as well as the geometry of the Universe. Its study can therefore bring higher constraints on the origin of the current accelerated expansion of the Universe that led to the notion of dark energy. **In the absence of systematic errors, weak lensing is even recognised as the single most constraining probe of dark energy. As such, its analysis is one of the main science drivers for both LSST and Euclid**. 

**Two main requirements are essential for using cosmic shear: accurately measuring galaxy shapes and galaxy redshifts. Given the wealth and volume of forthcoming data, these aspects present a set of new challenges, for which machine learning techniques are particularly well suited.**

For example, the sheer volume of produced data requires the development of new types of analyses that allow more efficient processing. Plus novel complexities arise. To address these challenges, our group has started to develop an approach based on Bayesian neural networks (BNNs, see for example [1]). The BNNs offer a formalism to quantify and propagate uncertainties associated with deep neural networks models and also with the data itself, which are both key for cosmological analyses. 

To give an idea, as more and more galaxies and stars populate the images in deep surveys, the local density increases and the projected objects naturally overlap. This phenomenon, referred to as blending, impedes the ability to properly measure the shapes and photometry of individual objects and  will affect more than 60% of the galaxies in LSST. To address this issue, deep learning brings a possible solution, with an efficient use of the joint multi-band processing of LSST and Euclid images. The images are fed to a BNN to separate overlapping galaxies before measuring their shape and this approach brings an improvement to the use of one of the surveys alone (as it brings the complexity but also the power of a multi-resolution and multiwavelength approach to the problem). We have demonstrated the feasibility of this approach in a configuration with several simulated galaxies per image ([2]) and developed several architectures aiming at the deblending of images in our group ([2], [3]).

Another aspect of the “blending problem” is the misdetection of sources : as galaxies overlap, under given conditions galaxies can play hide and seek. Consequences are two-fold : 

- The detected object has contaminated photometry & shape measurements 
- The number of objects associated to a given redshift is biased.

As the sources are not correctly detected the blended scene flag is not even raised and can lead for some algorithms to the disregarding of the problem altogether. This is what is called an unrecognized blend. This leads to several biases impacting both clustering and cosmic shear analyses that can result in measurable effects on the derived cosmological parameters. 

**The goal of this PhD project is to bring a new approach of detection to account for the probability of misdetected galaxies, keeping the number of detected objects itself as a random variable, leading to a probabilistic treatment of sources. This will be integrated with other elements formerly developed by our group or the DESC collaboration to bring a proof of principle of a pure Bayesian pipeline for the probabilistic determination of the cosmic shear on a patch of sky (see [5] and [6])**. The principle here is not new as hierarchical Bayesian approaches have been thought of for shear analyses (see for example [7] or [8]), although they have never been implemented. They moreover currently raise much attention in the DESC collaboration, as a working group dedicated to Bayesian pipelines has been formed. 

**During the pre-thesis internship**, the main topic to pursue would be to enter the topic, familiarize with the existing architectures that have been developed in the group and get to a first treatment of a simulated field of galaxies for a probabilistic detection of sources.

##Local Context : 

From a local environment perspective, this PhD will occur in the scope of the AstroDeep project started in October 2019 at APC and that has started a follow up ANR funding in 2024. AstroDeep has been a pioneer in Bayesian deep learning techniques, with applications for handling blending in deep surveys, and simulation-based inference. The group has strong ties with the Rubin/LSST Dark Energy Science Collaboration (LSST-DESC) and the LSST Informatics & Statistics Science Collaboration (ISCC). The research will be conducted in connection with working groups from these collaborations.

If successful, the implications of this work could drastically reduce the bias on cosmic shear measurements and release an essential tool for observational cosmology to the community. Not to mention that **LSST and Euclid data are becoming available for science**, making these studies all the more interesting as the scientific environment will be extremely dynamic.

##Proposed research activities :

The research will build on our previous work on deblending galaxies and measuring galaxy parameters with modified variational autoencoders ([2], [3], past PhD of Bastien Arcelin and PhD in progress by Anna Preto). It will address the key question of unrecognized blends: missing a galaxy during the deblending process would bias the measurements on the other galaxies, as would, on the other way, considering as a galaxy what is pure noise in the images. A solution is not to decide deterministically the number of galaxies in a group, but keep it as a discrete probabilistic measure, and for each hypothesis measure the properties of each detected galaxy. New ways to represent this information will have to be defined, and existing software will have to be adapted.

The research will utilize both realistic simulated data, developed within relevant scientific collaborations like DESC, and data from recent surveys such as HSC, Rubin/LSST, and Euclid. A significant part of the work will involve comparing, selecting, adapting, and improving existing machine learning techniques, or developing new ones, to take into account and propagate uncertainties both on the number of objects and on their properties in a Bayesian analysis pipeline leading to a 3x2-pt analysis.

Bayesian deep learning techniques will be employed to account for uncertainties in the data and models. In addition to classical network architectures like convolutional networks and their Bayesian extensions, the student will explore variational autoencoders, transformers and attention mechanisms, physics-informed networks, and self-supervised training techniques like contrastive learning.

The student will also gain knowledge in cosmology, weak gravitational lensing, machine learning and massive astronomical data processing. The research is expected to produce production-grade software for combined cosmological analysis of large survey datasets. The skills and knowledge acquired during the PhD will enable the pursuit of a career in academia, focusing on cosmology or software engineering, as well as opportunities in the private sector.


[1] Tom Charnock, Laurence Perreault-Levasseur, François Lanusse, Bayesian Neural Networks, arXiv:2006.01490

[2] Bastien Arcelin, Cyrille Doux, Eric Aubourg, Cécile Roucelle, Deblending galaxies with Variational Autoencoders: a joint multi-band, multi-instrument approach, Monthly Notices of the Royal Astronomical Society, staa3062, https://doi.org/10.1093/mnras/staa3062 arXiv:2005.12039v1

[3] MADNESS Deblender Maximum A posteriori with Deep NEural networks for Source Separation, B. Biswas, E. Aubourg, A. Boucaud, A. Guinot, J. Lao, C. Roucelle, and the LSST Dark Energy Science Collaboration, under review by A&A https://hal.science/hal-04680436v1 see also B. Biswas PhD thesis 

[4] AstroCLIP: A Cross-Modal Foundation Model for Galaxies, L. Parker, F. Lanusse et al. arXiv:2310.034

[5] Porqueres, Natalia et al. (Feb. 2021a). “Bayesian forward modelling of cosmic shear data”. In: Monthly Notices of the Royal Astronomical Society 502.2. arXiv:2011.07722 [astro-ph], pp. 3035–3044. 
issn: 0035-8711, 1365-2966. doi: 10.1093/mnras/stab204. url: http://arxiv.org/abs/2011.07722.

[6] Porqueres, Natalia et al. (Dec. 2021b). “Lifting weak lensing degeneracies with a field-based likelihood”. en. In: Monthly Notices of the Royal Astronomical Society 509.3. Publisher: Oxford
Academic, pp. 3194–3202. issn: 0035-8711. doi: 10.1093/mnras/stab3234. url: https:
//dx.doi.org/10.1093/mnras/stab3234.

[7] Hansen, Derek et al. (July 2022). Scalable Bayesian Inference for Detection and Deblending in Astronomical Images. arXiv:2207.05642 [astro-ph]. doi: 10.48550/arXiv.2207.05642.
url: http://arxiv.org/abs/2207.05642

[8] Schneider, Michael D. et al. (July 2015). “HIERARCHICAL PROBABILISTIC INFERENCE
OF COSMIC SHEAR”. en. In: The Astrophysical Journal 807.1. Publisher: The American
Astronomical Society, p. 87. issn: 0004-637X. doi: 10.1088/0004-637X/807/1/87. url:
https://dx.doi.org/10.1088/0004-637X/807/1/87
