---
layout: publication
title: A GPU-Based High-Resolution Multi-Level Biomechanical Head-and-Neck Model for Validating Deformable Image Regsitration
authors: Jack Neylon, X. Sharon Qi, Ke Sheng, Robert Staton, Jason Pukala, Rafael Manon, Daniel A. Low, Patrick Kupelian, and Anand Santhanam
journal: Medical Physics
volume: 42
issue: 1
date: 2014-12-22
year: 2014
doi: https://doi.org/10.1118/1.4903504
link: /docs/2014-12-22-gpu-based-high-res-biomechanical-head-and-neck-model.pdf
---
**Purpose**

Validating the usage of deformable image registration (dir) for daily patient positioning is critical for adaptive radiotherapy (RT) applications pertaining to head and neck (HN) radiotherapy. The authors present a methodology for generating biomechanically realistic ground‐truth data for validating dir algorithms for HN anatomy by (a) developing a high‐resolution deformable biomechanical HN model from a planning CT, (b) simulating deformations for a range of interfraction posture changes and physiological regression, and (c) generating subsequent CT images representing the deformed anatomy.

**Methods**

The biomechanical model was developed using HN kVCT datasets and the corresponding structure contours. The voxels inside a given 3D contour boundary were clustered using a graphics processing unit (GPU) based algorithm that accounted for inconsistencies and gaps in the boundary to form a volumetric structure. While the bony anatomy was modeled as rigid body, the muscle and soft tissue structures were modeled as mass–spring‐damper models with elastic material properties that corresponded to the underlying contoured anatomies. Within a given muscle structure, the voxels were classified using a uniform grid and a normalized mass was assigned to each voxel based on its Hounsfield number. The soft tissue deformation for a given skeletal actuation was performed using an implicit Euler integration with each iteration split into two substeps: one for the muscle structures and the other for the remaining soft tissues. Posture changes were simulated by articulating the skeletal structure and enabling the soft structures to deform accordingly. Physiological changes representing tumor regression were simulated by reducing the target volume and enabling the surrounding soft structures to deform accordingly. Finally, the authors also discuss a new approach to generate kVCT images representing the deformed anatomy that accounts for gaps and antialiasing artifacts that may be caused by the biomechanical deformation process. Accuracy and stability of the model response were validated using ground‐truth simulations representing soft tissue behavior under local and global deformations. Numerical accuracy of the HN deformations was analyzed by applying nonrigid skeletal transformations acquired from interfraction kVCT images to the model's skeletal structures and comparing the subsequent soft tissue deformations of the model with the clinical anatomy.

**Results**

The GPU based framework enabled the model deformation to be performed at 60 frames/s, facilitating simulations of posture changes and physiological regressions at interactive speeds. The soft tissue response was accurate with a R2 value of >0.98 when compared to ground‐truth global and local force deformation analysis. The deformation of the HN anatomy by the model agreed with the clinically observed deformations with an average correlation coefficient of 0.956. For a clinically relevant range of posture and physiological changes, the model deformations stabilized with an uncertainty of less than 0.01 mm. 

**Conclusions**

Documenting dose delivery for HN radiotherapy is essential accounting for posture and physiological changes. The biomechanical model discussed in this paper was able to deform in real‐time, allowing interactive simulations and visualization of such changes. The model would allow patient specific validations of the dir method and has the potential to be a significant aid in adaptive radiotherapy techniques. 
