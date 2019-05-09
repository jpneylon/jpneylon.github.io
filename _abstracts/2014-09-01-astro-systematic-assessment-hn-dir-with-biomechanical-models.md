---
layout: abstract
title: A Systematic ASssessment of Head-and-Neck Deformable Image Regsitration Using High Resolution Biomechanical Models
authors: Anand Santhanam, Jack Neylon, R Staton, X. Sharon Qi, and Patrick Kupelian
conference: "ASTRO: 56th Annual Meeting"
journal: International Journal of Radiation Oncology Biology Physics
volume: 90
issue: 1
location: San Francisco, CA
date: 2014-09-14
---
**Purpose**

To develop an automated framework for 3D deformable image registration (DIR), register the pre-treatment CT scans to the planning CT scan and to quantify systematically the DIR accuracy using a biomechanical head and neck (BH&N) model for head and neck adaptive radiotherapy (ART).  

**Methods**

Patient specific BH&N models were generated from planning KVCT for eleven H&N cancer patientsin this analysis. For each patient, weekly kVCT scans were acquired during the course of the treatment. The BH&N model anatomy was developed using H&N KVCT dataset and the corresponding critical structure contours. While the bony anatomy was modeled as rigid body, the contoured muscle and soft tissue structures were modeled as a mass spring element with an elastic material property that corresponded to the underlying contoured anatomies. Given the clinical implementation, special consideration was taken to ensure that the computations were completed within 30-45 seconds, which is the interval between the time when the on-board imaging was acquired and the patient treatment was initiated. Using each of the biomechanical models, a set of 50 3D synthetic KVCT images (representing patient posture and physiological changes) was generated for deformations. The range of head and neck skeletal rotations along each of the three axes was set to be 5 degrees. In addition, biomechanically based PTV shrinkage was simulated up to a range of 75% of the original PTV volume. 
For DIR purposes, a GPU-based 3D optical flow was employed for registering the planning kVCT with their corresponding deformed synthetic 3D images. The ground truth for each of the 3D synthetic images was represented using a set of 4500 model-guided landmarks coupled with a landmark-based evaluation metric. 

**Results**

The in-house DIR tool achieved a near real-time speed (45 seconds) for registering each weekly kVCT with a planning CT. The average error in PTV, ipsilateral and contralateral parotids for posture changes was observed to be 0.6, 1.2 and 1.06 mm, respectively. The maximum DIR error was observed to be 2.3, 2.4 and 2.9 mm, respectively. For physiological changes, the average error was 3.4, 3.2, and 3.09 mm while the maximum error was 6.3, 8.5 and 8.9 mm, respectively.

**Conclusions**

Patient anatomic changes, including volume variation, center-of-mass displacement, and patient weight loss, etc. resulted in DIR errors that may lead to ART errors.  The proposed framework enables a systematic quantification of such errors.
