---
layout: abstract
title: Characterization of a Parameterized Image Similarity Cost Function for Automated Patient and Site Specific DIR Accuracy Optimizations
authors: Jack Neylon, Yugang Min, Katelyn Hasse, Daniel A. Low, and Anand Santhanam
conference: "AAPM: 58th Annual Meeting & Exhibition"
journal: Medical Physidcs
volume: 43
issue: 6
location: Washington, DC
date: 2016-07-31
---
**Purpose**

Clinical deformable image registration (DIR) accuracy is difficult to quantify, making validation and verification manual and time consuming. It has also been seen that DIR accuracy can be improved by patient and site specific optimization. We previously investigated a cost function to parameterize image similarity metrics (ISMs) and provide a quantifiable comparison of DIR performance. In this abstract, we characterize and optimize the cost function response (CFR) and correlation to target registration error (TRE) in a dense registration parameter space.

**Methods**

A validated head-and-neck biomechanical model was used to induce clinical deformations in patient kVCT data (source), outputting known ground truth deformation vector fields (DVFs) and simulated CTs of deformed anatomy (target). The source and target were registered repeatedly using an in-house optical flow DIR, systematically sampling the registration parameter space, and producing TREs and data volumes deformed according to the DIR DVF (warp). Normalized mutual information (NMI) was chosen as the test ISM. The cost function variables (CFV) were also systematically sampled to characterize their effect on the CFR. Sub-volume analysis was performed on the data, defined by structures of interest in the head-and-neck region.

**Results**

Strong inverse correlation was observed between the TRE and CFR when the data was subdivided around specific structures like the PTV, parotids, and mandible, reaching values of -0.95. The CFR slope changed by an order of magnitude by manipulating the CFV. Response and correlation were improved by adjusting on a structure specific basis. The CFR achieved a predominantly convex response, which should facilitate its use as an energy term in an optimization scheme.

**Conclusions**

Replacing the time consuming, manually placed landmark assessment methodology is necessary for patient and site specific registration optimization to be clinically feasible. The proposed cost function is a promising alternative for fast, fully automated DIR performance quantification.
