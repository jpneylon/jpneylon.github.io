---
layout: abstract
title: Distributed Multi-GPU Photon Beamlet Dose Calculation for Efficient Radiation Treatment Planning
authors: Ryan Neph, Cheng Ouyang, Jack Neylon, and Ke Sheng
conference: "AAPM: 60th Annual Meeting & Exhibition"
journal: Medical Physics
volume: 56
issue: 6
location: Nashville, TN
date: 2018-07-29
---
**Purpose**

To continuously improve plan quality, more beams and beamlets are considered in advanced treatment planning methods, adding substantially greater burden of accurate beamlet dose calculation even with conventional GPU implementation. We utilize a distributed network of multi-GPU compute nodes and develop a novel beamlet packing method based on spatial contexts to efficiently compute dose for a large number of beamlets using a highly optimized GPU Collapsed-Cone Convolution-Superposition (CCCS) algorithm. 

**Methods**

Our framework is compared with an existing single-GPU beamlet-based CCCS algorithm in lung and prostate anatomies for 1162 non-coplanar candidate photon beams, each consisting of up to 1600 active 5mm2 beamlets. An isotropic voxel size of 2.5mm is selected and all quality parameters are matched where possible. The calculation time using one GPU, and two GPUs distributed across one, two, and three networked nodes is measured. In addition, percent-depth-dose (PDD) is compared with Monte Carlo calculated dose in a water phantom for a 6MV flattening-filter-free beam and 10cm2 field at 100cm source-surface-distance. 

**Results**

Analysis of the PDD curves indicate close dosimetric agreement of our algorithm with the Monte Carlo calculated dose distribution. Comparison with the existing single-GPU implementation reveals that our algorithm provides 39x speedup on 1 GPU; and more than 100x on 4 GPUs across 2 nodes. We observe a near-linear proportionality between the number of GPU nodes utilized and overall calculation time. Further profiling demonstrates scalability to a widely distributed network of compute nodes with very little overhead.

**Conclusion**

Development of a highly parallel, distributed, and accurate model-based beamlet dose calculation platform clears a major obstacle for clinical implementation of advanced treatment planning techniques such as multiple non-coplanar arc and automated 4pi treatment planning wherein the number of beamlets to be computed is several orders of magnitude larger than in conventional IMRT problems. 

