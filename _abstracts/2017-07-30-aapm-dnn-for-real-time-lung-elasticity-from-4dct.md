---
layout: abstract
title: A Deep Neural Network Approach for Near Real-Time Lung Tissue Elasticity Estimations from 4DCT Imaging
authors: Anand Santhanam, Katelyn Hasse, Yugang Min, Jack Neylon, and Daniel A. Low
conference: "AAPM: 59th Annual Meeting & Exhibition"
journal: Medical Physics
volume: vv
issue: ii
location: Denver, CO
date: 2017-07-30
---
**Purpose**

The focus of this work is to develop a machine learning strategy for performing near-real-time lung tissue elasticity estimations using only deformation maps that would typically be available from 4DCT lung images.

**Methods**

Our approach employs deep learning neural networks that learn the lung tissue elastic distributions for known lung deformations generated from 10 virtual lung phantoms representing normal, emphysematous, and tumor tissue within the lungs and 10 4DCT datasets with tissue elasticity estimated using a model guided approach. Voxels were then equally divided into training and test sets. A supervised learning approach was used for the deep learning process, where the elasticity for a set of voxels in the training set was taken as the label for the learning process. A Batch-wise Stochastic Gradient Descent method was employed for learning and optimizing a 7-layer deep neural network model with each layer consisting of 2000 interconnected neural units. For computation purposes, a set of 4 Nvidia Titan X GPUs were employed during the learning process. 

**Results**

Our results showed that the deep learning approach estimated the elasticity in the test set with 91.94±5.20% of voxels within 1 kPa of the ground-truth elasticity. Variations in the elasticity distribution (label), boundary deformation, and geometry were investigated with respect to their effect on the predicted tissue elasticity accuracy. For the 4DCT patient datasets, our learning process was able to generate the ground-truth elasticity at 92% accuracy. In addition, the methodology facilitated near real-time elasticity estimations. The computation time for the elasticity was near real-time.

**Conclusion**

Using machine learning techniques, the patient-specific lung tissue elasticity can be estimated from 4DCT patient datasets in real-time. Enabling such measurements within the radiotherapy setup facilitates multiple advancements in lung radiotherapy ranging from lung preserving radiotherapy treatment planning to treatment response monitoring. 
