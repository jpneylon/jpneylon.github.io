---
layout: publication
title: A Neural Network Approach for Fast, Automated Quantification of DIR
authors: Jack Neylon, Yugang Min, Daniel A. Low, and Anand Santhanam
journal: Medical Physics, Volume 44, Issue 8
date: 2017-05-05
doi: https://doi.org/10.1002/mp.12321
link: /docs/2017-05-05-neural-network-approach-for-fast-automated-quantification-of-dir.pdf
---
**Purpose**

A critical step in adaptive radiotherapy (ART) workflow is deformably registering the simulation CT with the daily or weekly volumetric imaging. Quantifying the deformable image registration accuracy under these circumstances is a complex task due to the lack of known ground‐truth landmark correspondences between the source data and target data. Generating landmarks manually (using experts) is time‐consuming, and limited by image quality and observer variability. While image similarity metrics (ISM) may be used as an alternative approach to quantify the registration error, there is a need to characterize the ISM values by developing a nonlinear cost function and translate them to physical distance measures in order to enable fast, quantitative comparison of registration performance.

**Methods**

In this paper, we present a proof‐of‐concept methodology for automated quantification of DIR performance. A nonlinear cost function was developed as a combination of ISM values and governed by the following two expectations for an accurate registration: (a) the deformed data obtained from transforming the simulation CT data with the deformation vector field (DVF) should match the target image data with near perfect similarity, and (b) the similarity between the simulation CT and deformed data should match the similarity between the simulation CT and the target image data. A deep neural network (DNN) was developed that translated the cost function values to actual physical distance measure. To train the neural network, patient‐specific biomechanical models of the head‐and‐neck anatomy were employed. The biomechanical model anatomy was systematically deformed to represent changes in patient posture and physiological regression. Volumetric source and target images with known ground‐truth deformations vector fields were then generated, representing the daily or weekly imaging data. Annotated data was then fed through a supervised machine learning process, iteratively optimizing a nonlinear model able to predict the target registration error (TRE) for given ISM values. The cost function for sub‐volumes enclosing critical radiotherapy structures in the head‐and‐neck region were computed and compared with the ground truth TRE values.

**Results**

When examining different combinations of registration parameters for a single DIR, the neural network was able to quantify DIR error to within a single voxel for 95% of the sub‐volumes examined. In addition, correlations between the neural network predicted error and the ground‐truth TRE for the Planning Target Volume and the parotid contours were consistently observed to be > 0.9. For variations in posture and tumor regression for 10 different patients, patient‐specific neural networks predicted the TRE to within a single voxel > 90% on average.

**Conclusions**

The formulation presented in this paper demonstrates the ability for fast, accurate quantification of registration performance. DNN provided the necessary level of abstraction to estimate a quantified TRE from the ISM expectations described above, when sufficiently trained on annotated data. In addition, biomechanical models facilitated the DNN with the required variations in the patient posture and physiological regression. With further development and validation on clinical patient data, such networks have potential impact in patient and site‐specific optimization, and stream‐lining clinical registration validation.
