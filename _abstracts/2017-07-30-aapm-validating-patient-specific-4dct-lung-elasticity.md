---
layout: abstract
title: Characterizing and Validating Patient-Specific High-Resolution Lung Elasticity from 4DCT Imaging
authors: Katelyn Hasse, Jack Neylon, Yugang Min, Dylan O'Connell, Daniel A. Low, and Anand Santhanam
conference: "AAPM: 59th Annual Meeting & Exhibition"
journal: Medical Physics
volume: vv
issue: ii
location: Denver, CO
date: 2017-07-30
---
**Purpose**

The purpose of this project is to perform patient-specific lung elastography for radiotherapy purposes using routinely acquired 4DCT lung scans and a biomechanical model.

**Methods**

A set of 24 anonymized patient 4DCT scans of the lungs were acquired, and end-inhalation and end-exhalation breathing phases were registered to each other using an in-house optical flow DIR algorithm. The registered displacement of each voxel was taken to be the ground-truth deformation. A GPU-based biomechanical simulation was generated from the patient 4DCT source datasets and was used as a forward model to solve the inverse elasticity problem. Displacements at the surface of the lungs were applied as boundary constraints for the model-guided lung tissue elastography, while the inner voxels were allowed to deform according to the linear elastic forces computed within the biomechanical model. The inverse elasticity problem was solved by iteratively modifying the tissue elasticity, deforming the biomechanical model, and comparing the model displacement with the ground-truth. Convergence in the elasticity estimation was documented when 95% of voxels were within 10% of maximum deformation or after 100 iterations. For validation, mid-exhalation breathing phase data was acquired for 5 patients and analyzed using the converged elasticity estimation. 

**Results**

Maximum lung deformation was observed to be between 6 and 31 mm. After analyzing 24 4DCT datasets, 90.358.16% of voxels converged within 10% of the maximum deformation. The results show that lung elasticity can be measured using routine-acquired clinical 4DCT scans. The validation datasets converged with 85.21 10.25% of voxels within 10% of maximum deformation.

**Conclusion**

By utilizing clinical 4DCT lung deformation data coupled with a biomechanical model, lung elastography was performed for 24 patient datasets and validated with 5 patient datasets. The regional lung elasticity information found here can be used to develop lung preserving radiotherapy plans to better preserve functional lung regions. 
