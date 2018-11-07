---
layout: abstract
title: A Systematic Quantification of Image Registration Accuracy Using High-Resolution Patient-Specific Biomechanical Head-and-Neck Models
authors: Jack Neylon, Yugang Min, X. Sharon Qi, Patrick Kupelian, and Anand Santhanam
conference: "NIH NIBIB Training Grantees Meeting"
journal: 
volume: 
issue: 
location: Bethesda, MD
date: 2014-05-20
---
**Purpose**

 Deformable image registration (DIR) plays a pivotal role in head and neck adaptive radiotherapy but a systematic validation of DIR algorithms has been limited by a lack of quantitative high-resolution ground-truth. We address this limitation by developing a GPU-based framework that provides a systematic DIR validation by generating (a) model-guided synthetic CTs representing posture and physiological changes, and (b) model-guided landmark-based validation.

**Method**

 The GPU-based framework was developed to generate massive mass-spring biomechanical models from patient simulation CTs and contoured structures. The biomechanical model represented soft tissue deformations for known rigid skeletal motion. Posture changes were simulated by articulating skeletal anatomy, which subsequently applied elastic corrective forces upon the soft tissue. Physiological changes such as tumor regression and weight loss were simulated in a biomechanically precise manner. Synthetic CT data was then generated from the deformed anatomy. The initial and final positions for one hundred randomly chosen mass elements from each internal contoured structure were recorded as ground truth data. The original CT and deformed synthetic CT were then registered using an optical flow based DIR. The process was automated to create 45 postures for several levels of tumor regression. The skull and cervical vertebrae were rotated between 4 and -4 degrees about each axis. Tumor volumes were systematically reduced up to 30%.

**Results**

 Each synthetic data creation took approximately 28 seconds of computation time. The number of landmarks per data set varied between two and three thousand. The validation method is able to perform sub-voxel analysis of the DIR, and report the results by structure, giving a much more in depth investigation of the error. This framework also allows a fast method for optimizing the registration parameters to minimize the resultant error on a patient specific basis. The in-house DIR tool achieved a near real-time speed (30 seconds) for registering each weekly kVCT with a planning CT. The average error in primary target volume, ipsilateral and contralateral parotids for posture changes was observed to be 0.6, 1.2 and 1.06 mm, respectively. The maximum DIR error was observed to be 2.3, 2.4 and 2.9 mm, respectively. For physiological changes, the average error was 3.4, 3.2, and 3.09 mm while the maximum error was 6.3, 8.5 and 8.9 mm, respectively

**Conclusions**

 We presented a GPU based high-resolution biomechanical head and neck model to validate DIR algorithms by generating CT equivalent 3D volumes with simulated posture changes and physiological regression.

[Poster](/docs/2014-05-nibib-poster.pdf)


