---
layout: abstract
title: A Machine Learning and Biomechanical Approach for Generating Lung 4DCT from a Breath-Hold 3DCT
authors: Anand Santhanam, Katelyn Hasse, Jack Neylon, Yugang Min, Percy lee, and Daniel A. Low
conference: "AAPM: 60th Annual Meeting & Exhibition"
journal: Medical Physics
volume: 56
issue: 6
location: Nashville, TN
date: 2018-07-29
---
**Purpose**

Lung radiotherapy treatment response is conventionally monitored mid- and post-treatment using 3DCTs, which does not quantify the changes in the 4D lung functional physiology and dynamics. We address this limitation by generating a 4DCT from a given end-expiration 3DCT.

**Methods**

We present a method that uses a deep neural network that outputs the 3D lung tissue elastic distribution and boundary conditions for a given CT dataset. Our approach employs a constrained Generalized Adversarial Neural Network (cGAN) that learns (a) the lung tissue elastic distributions, and (b) boundary conditions in a supervised manner. A set of 22 4DCT datasets were used for training. Once trained, the cGAN generated the label (or elasticity) for given data (breath hold CT) images. A set of 13 breath-hold CTs with known 4DCTs were used for this validation. The estimated elasticity was then validated using (a) direct comparison with the ground truth elasticity data using an L2-norm, (b) comparison of the deformation vector fields generated using the cGAN estimated elasticity with ground truth deformation vector fields, and (c) regenerating synthetic 4DCT and comparing with teh gorund -truth 4DCTs using 3 image similarity metrics: Mutual Information (MI), Structured Similarity Index (SSIM), and Normalized Cross Correlation (NCC).

**Results**

A direct comparison with the ground truth data showed that the deep learning approach estimated the 4D dunamics with a mean prediction error of 0.7±0.3 mm. 89% of the displacement vector fields matched the goruhd0truth displacements within 1 mm and 10% displacement error criteria. respoectively. In addition, the synthetic 4DCTs generated from the neurla network matched the ground-truth 4DCT images wit MI, SSI, and NCC values of 1.77, 0.89, and 0.97, respectively.

**Conclusion**

The results show that a machine learning based approach can be effective in predicting the 4D dynamics from a given breath-hold CT dataset.
