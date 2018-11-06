---
layout: publication
title: Near Real-Time Assessment of Anatomic and Dosimetric Variations for Heand-and-Neck Radiation Therapy Via GPU-Based Dose Deformation Framework
authors: X. Sharon Qi, Anand Santhanam, Jack Neylon, Yugang Min, Tess Armstrong, Ke Sheng, Robert Staton, Jason Pukala, Andrew Pham, Daniel A. Low, Steve P. Lee, Michael Steinberg, Rafael Manon, Allen Chen, and Patrick Kupelian
journal: International Journal of Radiation Oncology Biology Physics, Volume 92, Issue 2
date: 2015-01-27
year: 2015
doi: https://doi.org/10.1016/j.ijrobp.2015.01.033
link: /docs/2015-01-27-near-real-time-assessment-anatomic-dosimetric-variation-via-gpu-based-dose-deformation-framework.pdf
---
**Purpose**

The purpose of this study was to systematically monitor anatomic variations and their dosimetric consequences during intensity modulated radiation therapy (IMRT) for head and neck (H&N) cancer by using a graphics processing unit (GPU)-based deformable image registration (DIR) framework.

**Methods**

Eleven IMRT H&N patients undergoing IMRT with daily megavoltage computed tomography (CT) and weekly kilovoltage CT (kVCT) scans were included in this analysis. Pretreatment kVCTs were automatically registered with their corresponding planning CTs through a GPU-based DIR framework. The deformation of each contoured structure in the H&N region was computed to account for nonrigid change in the patient setup. The Jacobian determinant of the planning target volumes and the surrounding critical structures were used to quantify anatomical volume changes. The actual delivered dose was calculated accounting for the organ deformation. The dose distribution uncertainties due to registration errors were estimated using a landmark-based gamma evaluation.

**Results**

Dramatic interfractional anatomic changes were observed. During the treatment course of 6 to 7 weeks, the parotid gland volumes changed up to 34.7%, and the center-of-mass displacement of the 2 parotid glands varied in the range of 0.9 to 8.8 mm. For the primary treatment volume, the cumulative minimum and mean and equivalent uniform doses assessed by the weekly kVCTs were lower than the planned doses by up to 14.9% (P=.14), 2% (P=.39), and 7.3% (P=.05), respectively. The cumulative mean doses were significantly higher than the planned dose for the left parotid (P=.03) and right parotid glands (P=.006). The computation including DIR and dose accumulation was ultrafast (∼45 seconds) with registration accuracy at the subvoxel level.

**Conclusions**

A systematic analysis of anatomic variations in the H&N region and their dosimetric consequences is critical in improving treatment efficacy. Nearly real-time assessment of anatomic and dosimetric variations is feasible using the GPU-based DIR framework. Clinical implementation of this technology may enable timely plan adaptation and improved outcome.
