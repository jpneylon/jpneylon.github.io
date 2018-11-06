---
layout: abstract
title: Quantifying the Dose to Functional Lung Regions Using Patient-Specific Elasticity Distrubitions Estimated from a Deep Learning Approach
authors: Katelyn Hasse, Dylan O'Connell, Jack Neylon, Yugang Min, Percy Lee, Daniel A. Low, and Anand Santhanam
conference: "AAPM 2018: 60th Annual Meeting & Exhibition"
journal: Medical Physics, Volume 56, Issue 6
location: Nashville, TN
date: 2018-07-29
---
**Purpose**

The purpose of this work is to document the amount of dose delivered to functional lung regions during conventional treatment planning. 

**Methods**

A set of 20 patient planning CT scans of patients who underwent lung SBRT were retrospectively analyzed. The patients had a wide range of function, with COPD stage ranging from GOLD 0 – 4. Lung tissue elasticity was estimated using a deep learning approach that learned patient-specific lung tissue elastic distributions from the lung deformations measured between end-exhalation and end-inhalation scans. A set of 22 4DCT datasets were used for the training purpose. Once trained, the planning CT scans were then given as input to the neural network to determine the lung functional regions in terms of their elastic distribution. Treatment dose information was acquired and the dose and elasticity distributions were mapped to each other. The dose volume histograms were calculated for the full and functional lung volumes. Functional lung was considered to be those voxels of tissue with elasticity ranging between 4 and 8 kPa. For each patient, dose-volume and dose-function metrics, such as V5, V10, V20 and functional V5, V10, and V20 (denoted fV20), were calculated and compared.    

**Results**

For the patients included in this study, V5 ranged from 12.09 to 18.96, V10 ranged from 5.43 to 11.77, and V20 ranged from 1.96 to 4.46%. Functional metrics were also evaluated; fV5 ranged from 6.61 to 20.60, fV10 from 1.66 to 13.32, and fV20 ranged from 0.55 to 4.92%. These results indicate that for patients with earlier stage COPD, a substantial amount of functional tissue receives significant treatment dose.

**Conclusion**

Functional tissue as defined by 4DCT elastography receives varying amounts of dose during conventional radiotherapy treatment. Pre-treatment knowledge of regional lung function through 4DCT-elastography can be used to develop functional tissue-sparing radiotherapy treatment plans.

