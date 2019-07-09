---
layout: publication
title: "Parallel Beamlet Dose Calculation via Beamlet Contexts in a Distributed Multi-GPU Framework"
authors: Ryan Neph, Cheng Ouyang, John Neylon, Youming Yang, and Ke Sheng
journal: "Medical Physics"
acronym: MedPhys
volume: --
issue: -
date: 2019-06-10
year: 2019
doi: https://doi.org/10.1002/mp.13651
link: /docs/2019-06-10-parallel-beamlet-dose-calculation.pdf
---
**Purpose**

Dose calculation is one of the most computationally intensive, yet essential tasks in the
treatment planning process. With the recent interest in automatic beam orientation and arc trajectory
optimization techniques, there is a great need for more efficient model-based dose calculation algorithms
that can accommodate hundreds to thousands of beam candidates at once. Foundational work
has shown the translation of dose calculation algorithms to graphical processing units (GPUs), lending
to remarkable gains in processing efficiency. But these methods provide parallelization of dose
for only a single beamlet, serializing the calculation of multiple beamlets and under-utilizing the
potential of modern GPUs. In this paper, the authors propose a framework enabling parallel computation
of many beamlet doses using a novel beamlet context transformation and further embed this
approach in a scalable network of multi-GPU computational nodes.


**Methods**

The proposed context-based transformation separates beamlet-local density and TERMA into
distinct beamlet contexts that independently provide sufficient data for beamlet dose calculation. Beamlet
contexts are arranged in a composite context array with dosimetric isolation, and the context array is
subjected to a GPU collapsed-cone convolution superposition procedure, producing the set of beamletspecific
dose distributions in a single pass. Dose from each context is converted to a sparse representation
for efficient storage and retrieval during treatment plan optimization. The context radius is a new
parameter permitting flexibility between the speed and fidelity of the dose calculation process. A
distributed manager-worker architecture is constructed around the context-based GPU dose calculation
approach supporting an arbitrary number of worker nodes and resident GPUs. Phantom experiments
were executed to verify the accuracy of the context-based approach compared to Monte Carlo and a reference
CPU-CCCS implementation for single beamlets and broad beams composed by addition of
beamlets. Dose for representative 4p beam sets was calculated in lung and prostate cases to compare its
efficiency with that of an existing beamlet-sequential GPU-CCCS implementation. Code profiling was
also performed to evaluate the scalability of the framework across many networked GPUs.

**Results**

The dosimetric accuracy of the context-based method displays <1.35% and 2.35% average
error from the existing serialized CPU-CCCS algorithm and Monte Carlo simulation for beamletspecific
PDDs in water and slab phantoms, respectively. The context-based method demonstrates
substantial speedup of up to two orders of magnitude over the beamlet-sequential GPU-CCCS
method in the tested configurations. The context-based framework demonstrates near linear scaling
in the number of distributed compute nodes and GPUs employed, indicating that it is flexible enough
to meet the performance requirements of most users by simply increasing the hardware utilization.


**Conclusions**

The context-based approach demonstrates a new expectation of performance for beamlet-
based dose calculation methods. This approach has been successful in accelerating the dose calculation
process for very large-scale treatment planning problems - such as automatic 4p IMRT beam
orientation and VMAT arc trajectory selection, with hundreds of thousands of beamlets - in clinically
feasible timeframes. The flexibility of this framework makes it as a strong candidate for use in a
variety of other very large-scale treatment planning tasks and clinical workflows.
