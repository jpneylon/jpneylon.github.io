---
layout: abstract
title: Documenting Dose Delivery for Head-and-Neck Radiotherapy Using a GPU-Based Framework
authors: Anand Santhanam, Jack Neylon, X. Sharon Qi, Robert Staton, Ke Sheng, Daniel A. Low, and Patrick Kupelian
conference: "AAPM 2013: 55th Annual Meeting & Exhibition"
journal: Medical Physics, Volume 40, Issue 6
location: Indianapolis, IN
date: 2013-08-04
---
**Purpose**

To compute the delivered dose for head and neck (H&N) radiotherapy sccounting for the patient setup variations as well as physiologic changes during the entire treatment course. 

**Methods** 

The real‐time dose delivery documentation framework consisted of three components, a GPU based multi‐resolution optical flow based 3D registration framework, a GPU based local‐jocabian computation, and a GPU based dose accumulation framework. In addition, for validation purposes, a GPU based 3D gamma statistics was also employed. We evaluated the framework with ten H&N patients treated with simultaneous integrated boost on a TomoTherapy unit (Accuray Inc.). For every patient, a daily pre‐treatment megavoltage CT (MVCT) and weekly kilovoltage CT (KVCT) were acquired. The ability to account for different head and neck postures can be illustrated by observing the internal tissue deformations. The local‐Jacobian determinant for the PTVs and the critical structures were used to quantify anatomical volume changes for each week. The GPU‐accelerated dose accumulation determined the delivered mean/minimum/maximum dose, equivalent uniform dose (EUD), dose volume histograms (DVHs), as well as 3D gamma statistics comparing the delivered dose to the plan. 

**Results**

The ratios (and the standard deviations) between the delivered averaged minimum doses and the planned dose, were 0.73±0.14, 0.66±0.28 and 0.78±0.19 for PTV1 (the initial target volume), PTV2 (regions of involved nodes) and PTV3 (elective nodal areas) respectively. The framework achieved a run‐time of 30 sec for registering one KVCT with a planning KVCT, 0.1 sec for the forward dose accumulation and 10 sec for the 3D gamma statistical analyses making the system real‐time and an effective tool towards adaptive radiotherapy. 

**Conclusion**

The framework addresses the combined challenge of deforming the 3D anatomy using for treatment planning using the daily 3D image data and computing the delivered dose on the deformed planning 3D anatomy.
