---
layout: publication
title: Feasibility of Margin Reduction for Level II and III Planning Target Volume in Head-and-Neck Image-Guided Radiotherapy - Dosimetric Assessment via a Deformable Image Registration Framework
authors: X. Sharon Qi, Jack Neylon, Sumeyra Can, Robert Staton, Jason Pukala, Patrick Kupelian, and Anand Santhanam
journal: Current Cancer Therapy Reviews, Volume 10, Issue 4
date: 2014-05-20
doi: https://doi.org/10.2174/157339471004150407130229
link: /docs/2014-05-20-feasibility-margin-reductions_levels-ii-iii-hn-igrt-via-dir.pdf
---
**Purpose**

To improve normal tissue sparing for head-and-neck (H&N) image-guided radiotherapy (IGRT) by employing treatment plans with tighter margins for CTV 2 and 3, and documenting the delivered dose throughout the entire treatment course. 

**Methods**

Ten H&N cases treated with simultaneous integrated boost on a TomoTherapy unit (Accuray Inc.) were analyzed. Dose-limiting critical structures included brainstem, spinal cord, cochleae, parotid glands and mandible. The targets include the PTV1 (gross disease volume), PTV2 (next echelon nodal regions) and PTV3 (areas harboring subclinical disease). The standard margin plans (plan_ref) were generated using the standard margin of 3 mm to CTV1-3. Reduced margin plans (plan_0margin) using the CTV-to-PTV margin of zero for CTV2 and 3 were compared with plan_ref. All patients went through daily pre-treatment megavoltage CT (MVCT) and weekly kilovoltage CT (kVCT) scans. A GPU-based 3D image deformation/ visualization tool was developed to register the weekly kVCT scans with the planning CT scan. The deformation of each contoured structures was computed to account for non-rigid change in the patient setup. Calculation of the dose accumulation was performed to determine the delivered mean/minimum/maximum dose, dose volume histograms (DVHs), etc. 

**Results**

The averaged planned cord maximum doses in Plan_0margin were 7.6% lower, and the parotid mean doses were 18.9% lower than plan_Ref. No significant changes in D95 and D90 for the CTV2/3 cumulative doses in both reference and Plan_0margin were observed during the planning stage. Under kVCT guidance on TomoTherapy, for the reference plans, the averaged cumulative mean dose ratios during the entire treatment course were consistent within 5% and 1.5% of the planned mean doses for PTVs and CTVs, respectively. Interfraction anatomical changes introduced variations in delivered target doses that reduced the improved normal structure sparing observed in plan_0margin during the planning stage. For the tighter margin plans, the cumulative mean dose ratios were consistent within 4.3% and 2.3% of the planned mean doses for CTV2 and CTV3, respectively. Similar dose variations of the delivered dose were seen for the reference and tighter margin plans. However, the delivered maximum and mean doses for the cord were 20% and 10% higher than the planned doses; a 3.6% higher cumulative mean dose for the parotids was also observed for the delivered dose than the planned doses in both plans.

**Conclusions**

The GPU-based image framework enables real-time dose verification, accumulation and documentation. By imposing tighter CTV margins for level 2 and 3 targets for H&N irradiation, acceptable cumulative doses were achievable when coupled with weekly kVCT guidance while improving normal structure sparing. 
