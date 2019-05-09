---
layout: abstract
title: Sysetmatic Assessment of a Novel Image Similarity Parameterization Metric for Fully Automated Quantification of Deformable Image Registration Accuracy
authors: Jack Neylon, Patrick Kupelian, and Anand Santhanam
conference: "AAPM: 57th Annual Meeting & Exhibition"
journal: Medical Physics
volume: 42
issue: 6
location: Anaheim, CA
date: 2015-07-12
---
**Purpose**

To propose and test a cost function, which parameterizes image similarity metrics (ISMs) to provide a robust quantification of deformable image registration (DIR) accuracy. The gold standard for quantitatively assessing registration accuracy is manually placed landmarks. However, placing landmarks are time consuming, user dependent, and suffers from small sample size. ISMs provide a mathematical formulation for quantifying the similarity of two intensity fields but provide little value without proper context.

**Method**

We present a novel formulation for computing a normalized, reliable and robust ISM. We consider the given image pairs to be the source and target images, and the image deformed from the source using the deformation vector field (DVF) as the warp image. A variety of ISMs were calculated for three sets of images: source-target (IST), source-warp (ISW), and target-warp (ITW). For an ‘accurate’ registration, the target-warp pair should have high similarity (ITW approaches 1), while the source-target and source-warp similarities should be equal ((IST – ISW) approaches 0). Combining these expectations, a cost function was designed to measure the registration performance. To test the sensitivity of the proposed cost function, errors were introduced into the registration results by applying systematic perturbations to the DVF.

**Results**

We employed 10 head and neck biomechanical models for generating the image sets. The cost function had strong correlation to the L2 norm of the perturbation field, displaying sensitivity to errors in the registration. The best results were seen using normalized mutual information, with improved sensitivity achieved by optimizing the cost functions weighting factors between the two expectations.

**Conclusions**

The cost function proposed provides a method for quantifying registration accuracy using ISMs, displaying results as a single normalized value. This user-independent, mathematical evaluation allows fast and simple comparison between registrations and would be useful for automating an iterative optimization of registration parameters. 
