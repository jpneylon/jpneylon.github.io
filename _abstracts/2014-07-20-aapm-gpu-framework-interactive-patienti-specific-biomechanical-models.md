---
layout: abstract
title: A GPU Framework for Developing Interactive High-Resolution Patient-Specific Biomechanical Models
authors: Jack Neylon, X. Sharon Qi, Ke Sheng, Patrick Kupelian, and Anand Santhanam
conference: "AAPM: 56th Annual Meeting & Exhibition"
journal: Medical Physics
volume: 41
issue: 6
location: Austin, TX
date: 2014-07-20
---
**Purpose**

To develop a framework that can generate high resolution, patient specific biomechanical models from a given simulation CT and contoured structures, accelerated by GPU to run at interactive speeds, for addressing adaptive radiotherapy objectives.

**Method**

A Mass-spring-damping (MSD) model was generated from each simulation CT. The mass elements of the model were generated for every voxel of anatomy, and positioned in a deformation space on GPU memory. MSD connections were established between neighboring mass elements in a dense distribution. Contoured internal structures allowed control over elastic material properties of different tissues. Once the model was initialized in GPU memory, skeletal anatomy was actuated using rigid-body transformations, while soft tissues were governed by elastic corrective forces and constraints. During deformation integration, each mass element experienced a tensile force, shear force, and spring damping force.

**Results**

The model was validated by applying a known load to a soft tissue block and comparing the observed deformation to ground truth calculations from established elastic mechanics. Both local and global load experiments yielded results with a correlation coefficient R2 > 0.98 compared to ground truth. Models were generated for several anatomical regions. Head and neck models accurately simulated posture changes by rotating skeletal anatomy in three dimensions. Pelvic models were developed for realistic deformations when changing bladder volume. Thoracic models demonstrated breast deformation due to gravity when changing treatment position from supine to prone. The GPU framework performed at greater than 30 iterations per second for over 1 million mass elements with up to 26 MSD connections each.

**Conclusions**

Realistic simulations of site-specific, complex posture and physiological changes were simulated at interactive speeds using actual patient data. Incorporating such a model with live patient tracking would facilitate real time assessment of variations of the actual anatomy and delivered dose for adaptive intervention and re-planning.

