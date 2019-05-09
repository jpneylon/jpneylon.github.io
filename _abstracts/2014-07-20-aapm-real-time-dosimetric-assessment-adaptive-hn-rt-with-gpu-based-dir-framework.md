---
layout: abstract
title: Real-Time Dosimetric Assessment for Adaptive Head-and-Neck Treatment Via a GPU-Based Deformable Image Registration Framework
authors: X. Sharon Qi, Jack Neylon, A Chen, Daniel A. Low, Patrick Kupelian, M Steinberg, and Anand Santhanam
conference: "AAPM: 56th Annual Meeting & Exhibition"
journal: Medical Physics
volume: 41
issue: 6
location: Austin, TX
date: 2014-07-20
---
**Purposes**

To systematically monitor anatomic variations and their dosimetric consequences during head-and-neck (H&N) radiation therapy using a GPU-based deformable image registration (DIR) framework. 

**Methods**

Eleven H&N IMRT patients comprised the subject population. The daily megavoltage CT and weekly kVCT scans were acquired for each patient. The pre-treatment CTs were automatically registered with their corresponding planning CT through an in-house GPU-based DIR framework. The deformation of each contoured structure was computed to account for non-rigid change in the patient setup. The Jacobian determinant for the PTVs and critical structures was used to quantify anatomical volume changes. Dose accumulation was performed to determine the actual delivered dose and dose accumulation. A landmark tool was developed to determine the uncertainty in the dose distribution due to registration error.

**Results**

Dramatic interfraction anatomic changes leading to dosimetric variations were observed. During the treatment courses of 6-7 weeks, the parotid gland volumes changed up to 34.7%, the center-of-mass displacement of the two parotids varied in the range of 0.9-8.8mm. Mean doses were within 5% and 3% of the planned mean doses for all PTVs and CTVs, respectively. The cumulative minimum/mean/EUD doses were lower than the planned doses by 18%, 2%, and 7%, respectively for the PTV1. The ratio of the averaged cumulative cord maximum doses to the plan was 1.06±0.15. The cumulative mean doses assessed by the weekly kVCTs were significantly higher than the planned dose for the left-parotid (p=0.03) and right-parotid gland (p=0.006). The computation time was nearly real-time (~ 45 seconds) for registering each pre-treatment CT to the planning CT and dose accumulation with registration accuracy (for kVCT) at sub-voxel level (<1.5mm).

**Conclusions**

Real-time assessment of anatomic and dosimetric variations is feasible using the GPU-based DIR framework. Clinical implementation of this technology may enable timely plan adaption and potentially lead to improved outcome. 
