---
layout: abstract
title: Investigating the Minimum Scan Parameters Required to Generate Free-Breathing Fast-Helical CT Scans Without Motion Artifacts
authors: David Thomas, J Tan, Jack Neylon, Tai Dou, Shyam Jani, James Lamb, and Daniel A. Low
conference: "AAPM: 56th Annual Meeting & Exhibition"
journal: Medical Physics
volume: 41
issue: 6
location: Austin, TX
date: 2014-07-20
---
**Purpose**

A recently proposed 4D-CT protocol uses deformable registration of free-breathing fast-helical CT scans to generate a breathing motion model. In order to allow accurate registration, free-breathing images are required to be free of doubling-artifacts, which arise when tissue motion is greater than scan speed. This work identifies the minimum scanner parameters required to successfully generate free-breathing fast-helical scans without doubling-artifacts. 

**Methods**

10 patients were imaged under free breathing conditions 25 times in alternating directions with a 64-slice CT scanner using a low dose fast helical protocol. A high temporal resolution (0.1s) 4D-CT was generated using a patient specific motion model and patient breathing waveforms, and used as the input for a scanner simulation. Forward projections were calculated using helical cone-beam geometry (800 projections per rotation) and a GPU accelerated reconstruction algorithm was implemented. Various CT scanner detector widths and rotation times were simulated, and verified using a motion phantom. Doubling-artifacts were quantified in patient images using structural similarity maps to determine the similarity between axial slices. 

**Results**

Increasing amounts of doubling-artifacts were observed with increasing rotation times > 0.2s for 16x1mm slice scan geometry. No significant increase in doubling artifacts was observed for 64x1mm slice scan geometry up to 1.0s rotation time although blurring artifacts were observed >0.6s. Using a 16x1mm slice scan geometry, a rotation time of less than 0.3s (53mm/s scan speed) would be required to produce images of similar quality to a 64x1mm slice scan geometry. 

**Conclusion**

The current generation of 16 slice CT scanners, which are present in most Radiation Oncology departments, are not capable of generating free-breathing sorting-artifact-free images in the majority of patients. The next generation of CT scanners should be capable of at least 53mm/s scan speed in order to use a fast-helical 4D-CT protocol to generate a motion-artifact free 4D-CT.

