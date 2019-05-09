---
layout: abstract
title: Applications of Biomechanical Modeling in Adaptive Radiotherapy
authors: Jack Neylon
conference: "UCLA Biomedical Physics Symposium"
journal:
volume: 
issue: 
location: Los Angeles, CA
date: 2015-05-01
---
**Introduction**

The estimated number of new head and neck cancer cases in the U.S. for 2014 was 42,440 (National Cancer Institute). The major obstacle to delivering tumoricidal radiation doses is the resultant normal tissue toxicity leading to a reduction in the body’s normal function. A typical treatment course delivers the radiation daily over several weeks, but a patient’s anatomy is not static. Weight loss, patient positioning, respiratory and cardiac motion, and tumor regression all contribute to changing patient anatomy from day to day. Error margins are built into the treatment plan to account for these uncertainties and ensure that the diseased tissue is receiving the full prescription dose. Expanded error margins also increase the exposure of healthy tissues, which can lead to side effects and diminished quality of life. This risk can be reduced if the treatment plan is optimized to the daily patient anatomy, using adaptive radiation therapy (ART). An effective solution is to biomechanically model the patient’s changing anatomy.
Biomechanical models developed from actual patient computed tomography (CT) or magnetic resonance (MR) imaging can provide a subject specific physiological and musculoskeletal simulation. Physics-based methods allow for a broad array of simulations, from gross posture changes to subtle deformations like tumor regression. However, the computation time for complex simulations can take minutes to hours on a CPU. My research is focused on improving adaptive radiation therapy (ART) based cancer treatments by developing computational organ models accelerated by GPU architecture, which allows more sophisticated treatment simulations while improving the computational performance towards interactive speeds. 

**Methods**

A GPU-based biomechanical model was developed using a mass-spring-damper system where each mass represents a voxel from a patient CT scan. The physics of the model run entirely on GPU in a multi-level algorithm. Level 1 determines external impulses, such as user driven musculoskeletal motion. Level 2 identifies the contact forces between the internal structures, such two abutting organ surfaces. Level 3 resolves the internal forces of individual structures. 
Accurately modeling the elasticity of tissues is particularly important in cancer therapy. Historically, soft tissues have been modeled using linear elastic properties for simplicity, as is done in the current model. However, for large strains and deformations, most biological tissues are hyper-elastic, and exhibit a nonlinear response. Current work focuses on expanding the model to a multi-GPU framework which would provide the computational power to solve the nonlinear equations necessary to incorporate hyper-elastic properties into the model. 
A framework to update the patient-specific hyper-elastic biomechanical head & neck model using quantitative 3D surface imaging is also in development for documenting inter-fraction motion during radiotherapy. During treatment, the patient position will be tracked using 3D optical surface imaging. A GPU algorithm will be required to process the optical information, register the surface with the model, and propagate observed motion to the model for patient position tracking and dose estimations. The point cloud from the optical imaging will serve as control points on the model surface, providing the external impulses handled in Level 1 of the algorithm.

**Results**

The mass-spring-damper system was able to achieve interactive speeds (>30 fps) on a single GPU for a model with approximately 1.5 million masses and over 25 million springs, while maintaining stability and realistic biomechanics. This type of model is exceedingly versatile and has many applications in the medical field in addition to cancer therapy, such as surgical training, trauma simulation, and deformable image registration (DIR) validation. 
Results of a DIR validation study using the model were recently published. The biomechanical model simulated a spectrum of posture and physiological changes, creating nearly 300 unique anatomies for each of 10 clinical patient CT scans. The registration results were then compared to the known deformations produced by the model. 

**Conclusion**

A biomechanical model framework is in development to track patient positioning and dose accumulation for head and neck cancer patients. On a multi-GPU architecture, this model will run sophisticated hyper-elastic simulations, updated at interactive speeds using both 3D optical imaging and cone-beam CT imaging. This proposed workflow would provide important and novel clinical information not currently available to facilitate adaptive radiotherapy.

