---
layout: page
title: Postdocs at APC and CEA
permalink: jobs/postdocs-apc-cea/
subtitle: Multiple Postdoctoral Positions in Paris on Probabilistic Modeling and Analysis for Cosmology
---

- _start date_: As early as April 2025, and no later than Fall 2026
- _application deadline_ : 15/12/2025
- _duration_: 24 months
- _contact_: [jobs@astrodeep.net](mailto:jobs@astrodeep.net?subject=Postdoctoral positions at APC and CEA)

### Context

The ANR-funded AstroDeep² project, jointly led by the Astroparticle and Cosmology Laboratory (APC, Université Paris Cité) and the CosmoStat Laboratory at CEA Paris-Saclay, aims to develop new probabilistic and differentiable modeling and analysis techniques for the optimal exploitation of deep, wide-field astronomical surveys such as Euclid and Rubin/LSST. 
Its goal is to unlock the full information content of Stage IV imaging surveys by enabling end-to-end, field-level cosmological inference (from cosmology to pixels) through forward modeling, simulation-based inference (SBI), and differentiable simulation. The project will tackle challenging issues such  as enabling robust photo-z and shape estimation even under severe blending through advances in multimodal architectures, and developing probabilistic galaxy cataloguing for fully Bayesian shear pipelines that rigorously propagate uncertainties into downstream cosmological inference. 

As part of this project, we are recruiting **two postdoctoral researchers, one at CEA Paris-Saclay, one at APC**, to join a vibrant interdisciplinary team at the interface of cosmology, statistics, and machine learning.

### Main Research Directions

**The two postdoctoral researchers will contribute to one or more of the following complementary research directions, depending on their expertise and interests**. Together, these efforts aim to build a unified, differentiable, and probabilistic modeling framework for cosmological inference and address key systematic effects.


**Differentiable Programming for Cosmological Simulations**: This direction focuses on developing end-to-end differentiable models of cosmic structure formation using modern JAX-based tools such as JaxPM and jax-cosmo. The goal is to create fast, GPU-accelerated forward models capable of simulating weak-lensing and large-scale structure observables while retaining full differentiability with respect to cosmological parameters. The postdoctoral researcher will:

- Extend differentiable particle-mesh simulations (e.g. survey realism, systematics modeling)
- Explore hybrid physics-neural approaches, combining physical solvers with neural surrogates to improve accuracy and accelerate inference.

**Pixel-Level Forward Modeling**: This direction targets the measurement challenges at the image level (such as blending, shear estimation) by leveraging a combination of deep learning, differentiable programming, and probabilistic modeling. Building on the JAX-GalSim framework and recent advances in differentiable image rendering, the postdoctoral researcher will:

- Develop pixel-level generative models of galaxy populations to perform Bayesian shape and flux inference under realistic observing conditions.
- Combine multi-band, multi-instrument data to produce consistent uncertainty estimates and posterior samples for each object.

**Advanced Sampling Techniques for High-Dimensional Posteriors**: The third axis focuses on the development of novel probabilistic inference methods tailored to high dimensionality and non-Gaussianity Bayesian posteriors. The postdoctoral researcher will:

- Explore advanced sampling algorithms (e.g., annealed HMC, score-based diffusion samplers, or flow-matching approaches) to enable scalable posterior exploration in large-parameter spaces.
- Build a modular probabilistic inference engine integrated with the differentiable simulation and forward-modeling pipelines developed in the other work packages.

**Multimodal Architectures for Deblending and Galaxy Property Measurement**: This direction focuses on developing machine learning models that ingest multimodal data (imaging + spectroscopy). Building on prior work (e.g., DebVader, Arcelin, MADNESS, Biswas), the aim is self-supervised representation learning that captures shared and modality-specific galaxy physics, enabling robust photo-z and source identification for heavily blended scenes. The postdoctoral researcher will:

- Explore and benchmark multimodal architectures (e.g., MoE, BMVAE) for deblending and inference.
- Specialize models for key galaxy properties (photo-z, shapes, fluxes, morphology).
- Curate datasets for training and evaluation of generalization and uncertainty calibration.

**Probabilistic Cataloguing of Galaxies**: This direction targets biases from unrecognized blends in shear analyses by casting detection and measurement as a fully Bayesian problem. The goal is to construct probabilistic galaxy catalogues in which both object properties and object counts are modeled as random variables, and to propagate these uncertainties through downstream cosmological inference. The postdoctoral researcher will:

- Define data structures for catalogues with explicit density representations over galaxy properties and counts.
- Integrate catalogue outputs into end-to-end Bayesian shear pipelines, ensuring uncertainty propagation to the final inference.

### Qualifications

We welcome applicants with diverse backgrounds in astrophysics, cosmology, statistics, or machine learning, who are motivated to advance the frontiers of probabilistic and differentiable modeling for large-scale cosmological data analysis. Candidates should hold (or be close to completing) a PhD in one of these or closely related fields.

We are looking for individuals who have experience in one or more of the following areas:

- Differentiable simulations or physics codes: Experience with JAX, PyTorch, TensorFlow, or similar frameworks; familiarity with N-body or particle-mesh simulations; interest in developing differentiable or GPU-accelerated physical models.
- Image-level forward modeling and analysis: Background in astronomical image processing, weak lensing, or deblending; experience with image simulation frameworks (e.g. GalSim).
- Probabilistic inference and Bayesian computation: Strong foundation in Bayesian statistics, simulation-based inference, or Monte Carlo and variational methods; familiarity with modern samplers such as HMC, NUTS, diffusion- or flow-based samplers; interest in scalable inference for high-dimensional posteriors.
- Probabilistic neural networks architectures: Strong background in Deep Learning and probabilistic modeling.

Additional desired qualifications:

- Strong programming skills in Python and collaborative software development (Git/GitHub, CI/CD, open-source practices).
- Demonstrated ability to conduct independent research and contribute to collaborative, interdisciplinary projects.
- Excellent written and oral communication skills in English.
- Prior experience with large astronomical collaborations (e.g. LSST DESC, Euclid) is an asset but not required.

###Environment

####AstroDeep Team at APC (Université Paris Cité, Paris)

The AstroDeep team is hosted at the Astroparticle and Cosmology Laboratory (APC), located in central Paris within a vibrant scientific and cultural environment. APC is a leading French research institute in astrophysics, cosmology, and astroparticle physics, bringing together scientists working across theory, observation, and instrumentation. The team is deeply involved in international collaborations such as Euclid and the Vera C. Rubin Observatory (LSST), and plays a leading role in the LSST Dark Energy Science Collaboration (DESC) through contributions to Bayesian pipelines and simulation-based inference for cosmology.

#### CosmoStat Group at CEA Paris-Saclay

The CosmoStat Laboratory is located at CEA Paris-Saclay, about 20 km south of Paris, in close proximity to several universities and major research centers. CosmoStat is a diverse and multidisciplinary group working at the intersection of cosmology, statistics, and data science. The team develops cutting-edge statistical and computational tools for the analysis of cosmological data and contributes to key international projects, including Euclid and LSST.

Both environments offer dynamic, collaborative, and family-friendly workplaces that value diversity, equity, and inclusion. We strongly encourage applications from women and other underrepresented groups in science. Employment benefits include comprehensive health coverage, retirement and parental leave, paid vacation and sick days, subsidised meals, public transport discounts, access to sports and cultural activities, and optional French language classes.

### Application Instructions

Applications should be sent to both Francois Lanusse and Eric Aubourg ([jobs@astrodeep.net](mailto:jobs@astrodeep.net?subject=Postdoctoral positions at APC and CEA)) and must include:

1. CV, including a publication list;
2. Summary of previous research (maximum 2 pages);
3. Research statement (maximum 2 pages) describing your interests and potential contributions to the project;
4. 3 letters of recommendations that should be received by the application deadline, sent directly at [jobs@astrodeep.net](mailto:jobs@astrodeep.net?subject=Recommandation for postdoctoral positions at APC and CEA)  

Early applications are encouraged. For full consideration, materials should be received by 15/12/2025. Informal inquiries about the position are welcome.



