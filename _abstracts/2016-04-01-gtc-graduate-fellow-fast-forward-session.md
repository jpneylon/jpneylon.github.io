---
layout: abstract
title: Graduate Fellow Fast-Forward Session - Interactive, Patient-Specific Hyper-Elastic Biomechanical Models in Radiotherapy
authors: Jack Neylon
conference: "NVIDIA's GPU Technology Conference"
journal: 
volume: 
issue: 
location: San Jose, CA
date: 2016-04-01
---
**Abstract**

A major portion of my dissertation work has been developing interactive, patient-specific biomechanical models for radiotherapy purposes.

For these models to be clinically useful, they must be high resolution, patient specific, robust, and accurate. On top of all that, they need to be fast.  
Want to capture the volumetric information from individual patient CTs

1. We aimed to utilize the volumetric information from patient's planning CTs. Instantiated the model with a one-to-one correspondence between its elements and the CT voxels. Pre-processing step ~20s 

2. Then perform a nearest neighbor search to establish a volumetric mesh of up 26 connections about each element. Meshing performed in approximately 2 us/element.

3. Incorporate the contoured structures to segment the model and allow targeted control. User can directly manipulate the skeletal (rigid) anatomy.

4. Soft tissues then deform according to internal corrective forces calculated from a physics based material model

5. Can also simulate volume changes by altering the magnitude of the rest state vectors. Tumor regression by altering only the tumor's internal connections

6.Weight loss by reducing the connections of all generic soft tissues. Fast re-meshing (2 us/element) allows the incorporation of induced deformations into the rest state. So regressing the tumor doesn't contribute to the strain/force of a subsequent head rotation

7. Main application so far has been validation of deformable image registration algorithms. Clinical DIR hard to validate due to a lack of ground truth data. For any patient we can systematically create a suite of possible deformation and output simulated CTs with a known deformation vector field for quantifying DIR performance. 

Initially developed with linear elasticity, for simplicity and speed. Decent approximation for small deformations, but moving forward, a hyper-elastic material model more accurately describes soft tissue response.

8. One area we've expanded into is breast elastography and immobilization. Breast may undergo large deformation from day to day, immobilization is important to obtain reproducible geometry for treatment. Using the model for prototype testing and patient specific planning.
