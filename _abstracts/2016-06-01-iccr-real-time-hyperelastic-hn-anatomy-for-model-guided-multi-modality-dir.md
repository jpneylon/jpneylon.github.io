---
layout: abstract
title: Real-Time Hyper-Elastic Biomechanical Models of Head-and-Neck Anatomy for Model-Guided Multi-Modal Deformable Image Registrations
authors: Jack Neylon, X. Sharon Qi, Daniel A. Low, and Anand Santhanam
conference: "18th International Conference on the use of Computers in Radiation Therapy"
journal: 
volume: 
issue: 
location: London, UK
date: 2016-06-01
---
**Introduction**

Recent technological advancements have introduced a greater variety of imaging modalities to be incorporated into the clinical radiotherapy workflow. The daily acquired images may be a different modality than the planning kVCT. Clinical multi-modal deformable image registration (DIR) accuracy is difficult to quantify due to poor image quality of the daily imaging modalities (CBCT, MVCT), and the lack of known ground truth deformations for validation. The current gold standard is the physical distance between manually placed landmarks and the registration predictions. However, this process is time-consuming and subject to user-bias. In addition, intensity based DIR is difficult between modalities such as CT and MR, due to varying responses to different tissue types. To address this, a framework was developed to generate patient-specific, GPU-based biomechanical models. The model generated from the planning CT can be used to create ground truth deformation vector fields (DVF) by deforming to match the daily posture observed from the MR image. DIR accuracy can also be quantified by comparing the DIR and model generated DVFs, producing a confidence margin for the clinical registration.

[Poster](/docs/ICCR_2016_Poster_JNeylon-v4.pdf)
