---
layout: publication
title: A Non-Voxel-Based Dose Convolution/Superposition Algorithm Optimized for Scalable GPU Architectures
authors: Jack Neylon, Ke Sheng, Victoria Yu, Quan Chen, Daniel A. Low Patrick Kupelian, and Anand Santhanam
journal: Medical Physics
volume: 41
issue: 10
date: 2014-10-01
year: 2014
doi: https://doi.org/10.1118/1.4895822
link: /docs/2014-10-01-nvbb-cccs-gpu-algorithm.pdf
---
**Purpose**

Real‐time adaptive planning and treatment has been infeasible due in part to its high computational complexity. There have been many recent efforts to utilize graphics processing units (GPUs) to accelerate the computational performance and dose accuracy in radiation therapy. Data structure and memory access patterns are the key GPU factors that determine the computational performance and accuracy. In this paper, the authors present a nonvoxel‐based (NVB) approach to maximize computational and memory access efficiency and throughput on the GPU.

**Methods**

The proposed algorithm employs a ray‐tracing mechanism to restructure the 3D data sets computed from the CT anatomy into a nonvoxel‐based framework. In a process that takes only a few milliseconds of computing time, the algorithm restructured the data sets by ray‐tracing through precalculated CT volumes to realign the coordinate system along the convolution direction, as defined by zenithal and azimuthal angles. During the ray‐tracing step, the data were resampled according to radial sampling and parallel ray‐spacing parameters making the algorithm independent of the original CT resolution. The nonvoxel‐based algorithm presented in this paper also demonstrated a trade‐off in computational performance and dose accuracy for different coordinate system configurations. In order to find the best balance between the computed speedup and the accuracy, the authors employed an exhaustive parameter search on all sampling parameters that defined the coordinate system configuration: zenithal, azimuthal, and radial sampling of the convolution algorithm, as well as the parallel ray spacing during ray tracing. The angular sampling parameters were varied between 4 and 48 discrete angles, while both radial sampling and parallel ray spacing were varied from 0.5 to 10 mm. The gamma distribution analysis method (γ) was used to compare the dose distributions using 2% and 2 mm dose difference and distance‐to‐agreement criteria, respectively. Accuracy was investigated using three distinct phantoms with varied geometries and heterogeneities and on a series of 14 segmented lung CT data sets. Performance gains were calculated using three 256 mm cube homogenous water phantoms, with isotropic voxel dimensions of 1, 2, and 4 mm. 

**Results**

The nonvoxel‐based GPU algorithm was independent of the data size and provided significant computational gains over the CPU algorithm for large CT data sizes. The parameter search analysis also showed that the ray combination of 8 zenithal and 8 azimuthal angles along with 1 mm radial sampling and 2 mm parallel ray spacing maintained dose accuracy with greater than 99% of voxels passing the γ test. Combining the acceleration obtained from GPU parallelization with the sampling optimization, the authors achieved a total performance improvement factor of >175 000 when compared to our voxel‐based ground truth CPU benchmark and a factor of 20 compared with a voxel‐based GPU dose convolution method. 

**Conclusions**

The nonvoxel‐based convolution method yielded substantial performance improvements over a generic GPU implementation, while maintaining accuracy as compared to a CPU computed ground truth dose distribution. Such an algorithm can be a key contribution toward developing tools for adaptive radiation therapy systems.
