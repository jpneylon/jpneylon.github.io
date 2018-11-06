---
layout: abstract
title: Real-Time Assessment of Dosimetric Variations in Head-and-Neck Radiation Therapy
authors: X. Sharon Qi, Jack Neylon, Anand Santhanam, Yugang Min, Ke Sheng, Daniel A. Low, Steve P. Lee, Michael Steinberg, and Patrick Kupelian
conference: "ASTRO 2013: 55th Annual Meeting"
journal: International Journal of Radiation Oncology Biology Physics, Volume 87, Issue 2
location: Atlanta, GA
date: 2013-09-22
---
**Purposes**

 To assess the cumulative dose delivered for head-and-neck IMRT/IGRT treatment throughout the entire course. 

**Methods**

 Forty consecutive head-and-neck (H&N) patients treated with simultaneous integrated boost (SIB) on a TomoTherapy HD unit (Accuray Inc.) were considered in this study.  Treatment was performed using 2.0-2.1 Gy/fx in 25-33 fractions. For every patient, a daily pre-treatment megavoltage CT (MVCT) scan and a weekly long MVCT scan (covering the entire target volume) were acquired.  The targets and critical structures, such as PTVs, spinal cord, parotid glands, were delineated on the planning CT. A margin of 3 mm was used for the CTV-to-PTV expansion. A GPU-based 3D image deformation/registration tool was developed and employed for registering the weekly long MVCTs of each patient with their corresponding planning CT. The deformation of each contoured structures was computed to account for non-rigid change in the patient setup. The Jacobian value of the PTV and the critical structures was used to document anatomical volume changes for each week. A GPU based forward dose accumulation was performed to determine the delivered mean/minimum/maximum dose, equivalent uniform dose (EUD), dose volume histograms (DVHs), as well as 3D gamma statistics comparing the delivered dose to the plan. 

**Results**

 For a subgroup of 10 base-of-tongue/tongue and tonsil cases, cold spots were observed in the cumulative dose distributions for the targets compared to the plan. On average, the ratios (and the standard deviations) between the delivered averaged minimum doses and the planned dose, were 0.73±0.14, 0.66±0.28 and 0.78±0.19 for PTV1 (the initial target volume), PTV2 (regions of involved nodes) and PTV3 (elective nodal areas) respectively. The averaged maximum doses were consistent with the planned maximum doses within 1.6%, while the cumulative mean dose ratios were within 5% and 3% of the planned mean doses for all PTVs and CTVs respectively. The cumulative cord maximum and mean doses were 23% and 10% higher than the planned doses; at least one parotid gland received more than the planned mean doses by 4%.  During the treatment course, larger percent of target volume changes for the targets (up to 28%) and/or percent patient weight loss (up to 13.3%) associated with larger cumulative EUD variations up to 11, 22 and 8% for PTV1-3 were observed. The percentages of volume to fail the gamma criteria of 1% or 1mm for PTV1-3 were 28.2±10.99, 32.64±18.79, and 29.67±13.86. The tool achieved a run-time of 30 sec for registering one MVCT with a planning CT, 0.1 sec for the forward dose accumulation and 10 sec for the 3D gamma statistics computation. 

**Conclusions**

 Cumulative dose variations were documented using a GPU-based image framework with planned doses. The framework enables real-time dose verification and possible re-planning.   

