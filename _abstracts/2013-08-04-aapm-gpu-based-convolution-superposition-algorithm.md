---
layout: abstract
title: Establishing a Quantitative Relation Between the Spectrum-Sampling Rate on the Dose Distrubtion Accuracy Using a GPU-Based Convolution/Superposition Algorithm
authors: Jack Neylon, Anand Santhanam, Ke Sheng, Daniel A. Low, and Patrick Kupelian
conference: "AAPM: 55th Annual Meeting & Exhibition"
journal: Medical Physics
volume: 40
issue: 6
location: Indianapolis, IN
date: 2013-08-04
---
**Purpose**

The focus of this work was to determine the quantitative relationship between the spectrum-sampling rate and the dose calculation accuracy of a GPUaccelerated convolution/superposition dose algorithm. 

**Methods**

The GPU-accelerated dose algorithm is a convolution/superposition that samples, in a hyper-spherical fashion, the volume surrounding a voxel of primary interaction. A set of 8 static phantoms and 14 deformable physics-based lung models were used for this study. The static phantoms provided a performance baseline to gauge the more clinically relevant dynamic lung dose delivery and dose accuracy. Respiration simulations used a simple sinusoidal breathing pattern to divide the inhalation and exhalation phases equally into 20 total breathing sub-phases. The spectrum sampling parameters used for the convolution were the azimuthal and elevation angles, and the radial step sampling surrounding the point of primary interaction. The angular sampling parameters were varied between 8 and 48 steps while the radial sampling parameter was varied between 1 mm to 10mm. The sampling combination of 48/48/1mm was taken as the ground truth. A γ-statistics based dose distribution agreement of greater than 99% of voxels in the calculation with γ(2%, 2mm)<1% and γ(1%, 1mm)<1% was documented.

**Results**

For γ (2%,2 mm) the sampling parameters of 8/8/1mm satisfied the criteria for both phantom and lungs, while γ (1%, 1mm), a sampling parameter of 8/8/1mm satisfied the criteria for phantoms and a sampling parameter of 12/12/1mm satisfied the criteria for lungs. The GPU implementation provided an additional acceleration of up to 70-80x, ~200x, and ~2000X for both the phantoms and lung models as compared to CPU implementation with sampling parameters of 8/8/1mm, 12/12/1mm, and 48/48/1mm, respectively. 

**Conclusion**

The relation between the spectrum-sampling rate and the dose accuracy was quantified using a GPU based dose convolution/superposition satisfying two different γ criteria. 
