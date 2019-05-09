---
layout: abstract
title: Feasibility and Quantitative Analysis of 4DCT-Based High Precision Lung Elastography
authors: Katelyn Hasse, Jack Neylon, Daniel A. Low, and Anand Santhanam
conference: "AAPM: 58th Annual Meeting & Exhibition"
journal: Medical Physidcs
volume: 43
issue: 6
location: Washington, DC
date: 2016-07-31
---
**Purpose**

The purpose of this project is to derive high precision elastography measurements from 4DCT lung scans to facilitate the implementation of elastography in a radiotherapy context.

**Methods**

4DCT scans of the lungs were acquired, and breathing stages were subsequently registered to each other using an optical flow DIR algorithm. The displacement of each voxel gleaned from the registration was taken to be the ground-truth deformation. These vectors, along with the 4DCT source datasets, were used to generate a GPU-based biomechanical simulation that acted as a forward model to solve the inverse elasticity problem. The lung surface displacements were applied as boundary constraints for the model-guided lung tissue elastography, while the inner voxels were allowed to deform according to the linear elastic forces within the model. A biomechanically-based anisotropic convergence magnification technique was applied to the inner voxels in order to amplify the subtleties of the interior deformation. Solving the inverse elasticity problem was accomplished by modifying the tissue elasticity and iteratively deforming the biomechanical model. Convergence occurred when each voxel was within 0.5 mm of the ground-truth deformation and 1 kPa of the ground-truth elasticity distribution. To analyze the feasibility of the model-guided approach, we present the results for regions of low ventilation, specifically, the apex. 

**Results**

The maximum apical boundary expansion was observed to be between 2 and 6 mm. Simulating this expansion within an apical lung model, it was observed that 100% of voxels converged within 0.5 mm of ground-truth deformation, while 91.8% converged within 1 kPa of the ground-truth elasticity distribution. A mean elasticity error of 0.6 kPa illustrates the high precision of our technique.

**Conclusion**

By utilizing 4DCT lung data coupled with a biomechanical model, high precision lung elastography can be accurately performed, even in low ventilation regions of the lungs. 
