---
layout: publication
title: Systematic Feasibility Analysis of a Quantitative Elasticity Estimation for Breast Anatomy Using Supine/Prone Postures
authors: Katelyn Hasse, Jack Neyluon, Ke Sheng, and Anand Santhanam
journal: Medical Physics
volume: 43
issue: 3
date: 2016-02-17
year: 2016
doi: https://doi.org/10.1118/1.4941745
link: /docs/2016-02-17-systematic-feasibility-quantitative-elasticity-breast-anatomy-supine-prone-posture.pdf
---
**Purpose**

Breast elastography is a critical tool for improving the targeted radiotherapy treatment of breast tumors. Current breast radiotherapy imaging protocols only involve prone and supine CT scans. There is a lack of knowledge on the quantitative accuracy with which breast elasticity can be systematically measured using only prone and supine CT datasets. The purpose of this paper is to describe a quantitative elasticity estimation technique for breast anatomy using only these supine/prone patient postures. Using biomechanical, high‐resolution breast geometry obtained from CT scans, a systematic assessment was performed in order to determine the feasibility of this methodology for clinically relevant elasticity distributions.

**Methods**

A model‐guided inverse analysis approach is presented in this paper. A graphics processing unit (GPU)‐based linear elastic biomechanical model was employed as a forward model for the inverse analysis with the breast geometry in a prone position. The elasticity estimation was performed using a gradient‐based iterative optimization scheme and a fast‐simulated annealing (FSA) algorithm. Numerical studies were conducted to systematically analyze the feasibility of elasticity estimation. For simulating gravity‐induced breast deformation, the breast geometry was anchored at its base, resembling the chest‐wall/breast tissue interface. Ground‐truth elasticity distributions were assigned to the model, representing tumor presence within breast tissue. Model geometry resolution was varied to estimate its influence on convergence of the system. A priori information was approximated and utilized to record the effect on time and accuracy of convergence. The role of the FSA process was also recorded. A novel error metric that combined elasticity and displacement error was used to quantify the systematic feasibility study. For the authors' purposes, convergence was set to be obtained when each voxel of tissue was within 1 mm of ground‐truth deformation. 

**Results**

The authors' analyses showed that a ∼97% model convergence was systematically observed with no‐a priori information. Varying the model geometry resolution showed no significant accuracy improvements. The GPU‐based forward model enabled the inverse analysis to be completed within 10–70 min. Using a priori information about the underlying anatomy, the computation time decreased by as much as 50%, while accuracy improved from 96.81% to 98.26%. The use of FSA was observed to allow the iterative estimation methodology to converge more precisely. 

**Conclusions**

By utilizing a forward iterative approach to solve the inverse elasticity problem, this work indicates the feasibility and potential of the fast reconstruction of breast tissue elasticity using supine/prone patient postures.
