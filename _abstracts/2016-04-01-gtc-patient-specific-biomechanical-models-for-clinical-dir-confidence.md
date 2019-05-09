---
layout: abstract
title: Patient-Specific Hyper-Elastic Biomechanical Models for Clinical DIR Confidence Quantification
authors: Jack Neylon, X. Sharon Qi, Yugang Min, and Anand Santhanam
conference: "NVIDIA's GPU Technology Conference"
journal: 
volume: 
issue: 
location: San Jose, CA
date: 2016-04-01
---
**Motivation**

Daily imaging modalities (CBCT, MVCT) typically suffer from poor image quality, or completely different tissue response (MR), making intensity based registration problematic. Furthermore, the accuracy of clinical multi-modal deformable image registration (DIR) is difficult to quantify. A framework was previously developed to validate a deformable registration algorithm by generating patient-specific, GPU-based biomechanical models from head-and-neck (HN) patient CT scans and creating clinically realistic ground truth deformations. We now aim to expand the model’s applicability to quantify DIR confidence for clinical registrations between the planning CT and daily positioning images.

**Methods**

By deforming the model to match the observed daily anatomy and creating a ground truth deformation vector field, DIR performance can be quantified by comparing the DIR and model generated DVFs, producing a confidence margin for the clinical registration. To validate the model deformations, registration was performed between the planning CT and final weekly kVCT of clinical patient data. The DVF for the bony anatomy was applied to the model created from the planning CT, after which the soft tissues were allowed to deform according to the elastic material model. The correlation was then calculated between the model anatomy and observed target anatomy.
The model was initially developed using a linear elastic material model, however, most biological tissues exhibit hyper-elastic response for larger deformations. Hyper-elasticity was implemented using a generalized Ogden material model. The model was integrated using a second order implicit Euler integration.

**Results**

The biomechanical model has been able to simulate significant tumor regression and posture changes, producing clinically realistic soft tissue deformations and kV quality simulated CT data. Posture changes were performed by controlling the skeletal anatomy. Frame by frame computations increased in computational cost compared to the previous linear elastic implementation, but expansion to a multi-GPU framework should allow the model to maintain an interactive frame rate > 30 fps.

**Conclusion**

A biomechanical modelling approach could effectively bridge the gap to facilitate multi-modal DIR, specifically between CT and MR where direct registration is not feasible. The ability to apply anatomical and physiological knowledge to the deformation could also improve the reliability of the daily deformation tracking for soft tissues, when utilizing lower quality modalities such as MVCT and CBCT.

[Poster](/docs/GTC_2016_Poster_JNeylon-DIR-v2.pdf)
