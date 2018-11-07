---
layout: publication
title: Modeling and Incorporating Cardiac-Induced Lung Tissue Motion in a Breathing Motion Model
authors: Ben White, Anand Santhanam, David Thomas, Yugang Min, James, Lamb, Jack Neylon, Shyam Jani, Sergio Gaudio, Subashini Srinivasan, Daniel Ennis, and Daniel A. Low
journal: Medical Physics
volume: 41
issue: 4
date: 2014-03-05
year: 2014
doi: https://doi.org/10.1118/1.4866888 
link: /docs/2014-03-05-modeling-cardiac-induced-lung-tissue-motion.pdf
---
**Purpose**

Thepurposeofthisworkistodevelopacardiac-inducedlungmotionmodeltobeintegrated into an existing breathing motion model

**Methods**

The authors’ proposed cardiac-induced lung motion model represents the lung tissue’s speciﬁc response to the subject’s cardiac cycle. The model is mathematically deﬁned as a product of a converging polynomial function h of the cardiac phase (c) and the maximum displacement  γ(  X0) of each voxel (  X0) among all the cardiac phases. The function h(c) was estimated from cardiac-gated MR imaging of ten healthy volunteers using an Akaike Information Criteria optimization algorithm. For each volunteer, a total of 24 short-axis and 18 radial planar views were acquired on a 1.5 T MR scannerduringaseriesof12–15sbreath-holdmaneuvers.Eachviewcontained30temporalframesof equal time-duration beginning with the end-diastolic cardiac phase. The frames in each of the planar views were resampled to create a set of three-dimensional (3D) anatomical volumes representing thoracic anatomy at different cardiac phases. A 3D multiresolution optical ﬂow deformable image registration algorithm was used to quantify the difference in tissue position between the end-diastolic cardiac phase and the remaining cardiac phases. To account for image noise, voxel displacements whose maximum values were less than 0.3 mm, were excluded. In addition, the blood vessels were segmented and excluded in order to eliminate registration artifacts caused by blood-ﬂow.

**Results**

The average cardiac-induced lung motions for displacements greater than 0.3 mm were found to be 0.86 ± 0.74 and 0.97 ± 0.93 mm in the left and right lungs, respectively. The average model residual error for the ten healthy volunteers was found to be 0.29±0.08 mm in the left lung and 0.38 ± 0.14 mm in the right lung for tissue displacements greater than 0.3 mm. The relative error decreased with increasing cardiac-induced lung tissue motion. While the relative error was > 60% for submillimeter cardiac-induced lung tissue motion, the relative error decreased to < 5% for cardiac-induced lung tissue motion that exceeded 10 mm in displacement.

**Conclusions**

The authors’ studies implied that modeling and including cardiac-induced lung motion would improve breathing motion model accuracy for tissues with cardiac-induced motion greater than 0.3 mm. 
