---
layout: publication
title: Fast Simulated Annealing and Adaptive Monte Carlo Sampling Based Parameter Optimization for Dense Optical Flow Deformable Image Registration of 4DCT Lung Anatomy
authors: Tai Dou, Yugang Min, Jack Neylon, David Thomas, Patrick Kupelian, and Anand Santhanam
journal: "SPIE Proceedings Volume 9786, Medical Imaging 2016: Image-Gudied Procedures, Robotic Interventions, and Modeling"
published: 2016-03-18
doi: https://doi.org/10.1117/12.2217194
link: /docs/2016-03-18-fast-simulated-annealing-adaptive-mc-parameter-optimization-optical-flow-dir.pdf
---
Deformable image registration (DIR) is an important step in radiotherapy treatment planning. An optimal input registration parameter set is critical to achieve the best registration performance with the specific algorithm. 

In this paper, we investigated a parameter optimization strategy for Optical-flow based DIR of the 4DCT lung anatomy. A novel fast simulated annealing with adaptive Monte Carlo sampling algorithm (FSA-AMC) was investigated for solving the complex non-convex parameter optimization problem. The metric for registration error for a given parameter set was computed using landmark-based mean target registration error (mTRE) between a given volumetric image pair. To reduce the computational time in the parameter optimization process, a GPU based 3D dense optical-flow algorithm was employed for registering the lung volumes. 

Numerical analyses on the parameter optimization for the DIR were performed using 4DCT datasets generated with breathing motion models and open-source 4DCT datasets. 

Results showed that the proposed method efficiently estimated the optimum parameters for optical-flow and closely matched the best registration parameters obtained using an exhaustive parameter search method. 
