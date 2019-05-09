---
layout: abstract
title: Systematic Feasibility Analysis of a Quantitative Elasticity Estimation for Breast Anatomy Using Supine/Prone Model Postures
authors: Katelyn Hasse, Jack Neylon, and Anand Santhanam
conference: "AAPM: 57th Annual Meeting & Exhibition"
journal: Medical Physics
volume: 42
issue: 6
location: Anaheim, CA
date: 2015-07-12
---
**Purpose**

The purpose of this project is to estimate an elasticity distribution of breast tissue using supine/prone patient postures. Using biomechanical high-resolution breast models, a systematic assessment was performed in order to determine the feasibility of using patient standard clinical CT data. 

**Methods**

A GPU-based framework was used to generate a mass-spring model with a hemispherical geometry to represent a breast in the prone position. The model was anchored to the base of the hemisphere mimicking the chest-wall/breast tissue interface. The model then was deformed with several ground-truth elasticity distributions. Both isotropic and anisotropic elasticity distributions were used to demonstrate a tumor's presence in the breast tissue. Solving the inverse elasticity problem was accomplished with a forward iterative approach by resetting the model to a non-deformed position and iteratively deforming it. A gradient-based iterative optimization scheme was used to update elasticity distribution in order to minimize the discrepancy between ground-truth and computed mechanical responses (displacement) for each voxel. For the purpose of our feasibility study, convergence was obtained when each voxel of tissue was within 1 mm of the ground-truth deformation. The model resolution was systematically varied to verify convergence at different volume representations.

**Results**

For a simulated hemisphere running at 200 deformations per second (dps) with about 100,000 mass elements and 26 mass-spring connections, convergence occurred within minutes for each elastic distribution. Using apriori information about the underlying anatomy, these elasticity distribution were estimated in half the computation time with the accuracy improving from 89% to 93%. Though the effective elasticity estimation varied slightly from the ground-truth, displacement magnitude difference was well within 0.1 mm.

**Conclusion**

By utilizing a forward iterative approach to solve the inverse elasticity problem, this work indicates the feasibility and potential of the fast reconstruction of breast tissue elasticity distribution using supine/prone postures. 
