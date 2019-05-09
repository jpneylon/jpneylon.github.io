---
layout: abstract
title: A GPU-Based Bethod for Validating Deformable Image Registration in Head-and-Neck Radiotherapy Using Biomechanical Modeling
authors: Jack Neylon, Yugang Min, X. Sharon Qi, Patrick Kupelian, and Anand Santhanam
conference: "AAPM: 56th Annual Meeting & Exhibition"
journal: Medical Physics
volume: 41
issue: 6
location: Austin, TX
date: 2014-07-20
---
**Purpose**

Deformable image registration (DIR) plays a pivotal role in head and neck adaptive radiotherapy but a systematic validation of DIR algorithms has been limited by a lack of quantitative high-resolution ground-truth. We address this limitation by developing a GPU-based framework that provides a systematic DIR validation by generating (a) model-guided synthetic CTs representing posture and physiological changes, and (b) model-guided landmark-based validation.

**Method**

The GPU-based framework was developed to generate massive mass-spring biomechanical models from patient simulation CTs and contoured structures. The biomechanical model represented soft tissue deformations for known rigid skeletal motion. Posture changes were simulated by articulating skeletal anatomy, which subsequently applied elastic corrective forces upon the soft tissue. Physiological changes such as tumor regression and weight loss were simulated in a biomechanically precise manner. Synthetic CT data was then generated from the deformed anatomy. The initial and final positions for one hundred randomly chosen mass elements from each internal contoured structure were recorded as ground truth data. The original CT and deformed synthetic CT were then registered using an optical flow based DIR. The process was automated to create 45 synthetic CT datasets for a given patient CT. For instance, the head rotation was varied between 4 and -4 degrees along each axis, and tumor volumes were randomly reduced up to 30%.

**Results**

Each synthetic data creation took approximately 28 seconds of computation time. The number of landmarks per data set varied between two and three thousand. The validation method is able to perform sub-voxel analysis of the DIR, and report the results by structure, giving a much more in depth investigation of the error.

**Conclusions**

We presented a GPU based high-resolution biomechanical head and neck model to validate DIR algorithms by generating CT equivalent 3D volumes with simulated posture changes and physiological regression.

