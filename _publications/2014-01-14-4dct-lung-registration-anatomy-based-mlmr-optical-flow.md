---
layout: publication
title: 4DCT Lung Registration Using Anatomy-Based Multi-Level Multi-Resolution Optical Flow Analysis and Thin-Plate Splines
authors: Yugang Min, Jack Neylon, Amish Shah, Sanford Meeks, Percy Lee, Patrick Kupelian, and Anand Santhanam
journal: International Journal of Computer Assisted Radiology & Surgery, Volume 9, Issue 5
date: 2017-05-05
yeay: 2017
doi: https://doi.org/10.1007/s11548-013-0975-7
link: /docs/2014-01-14-4dct-lung-registration-anatomy-based-mlmr-optical-flow.pdf
---
**Purpose**

The accuracy of 4D-CT registration is limited by inconsistent Hounsfield unit (HU) values in the 4D-CT data from one respiratory phase to another and lower image contrast for lung substructures. This paper presents an optical flow and thin-plate spline (TPS)-based 4D-CT registration method to account for these limitations.

**Methods**

The use of unified HU values on multiple anatomy levels (e.g., the lung contour, blood vessels, and parenchyma) accounts for registration errors by inconsistent landmark HU value. While 3D multi-resolution optical flow analysis registers each anatomical level, TPS is employed for propagating the results from one anatomical level to another ultimately leading to the 4D-CT registration. 4D-CT registration was validated using target registration error (TRE), inverse consistency error (ICE) metrics, and a statistical image comparison using Gamma criteria of 1 % intensity difference in 2 mm<sup>3</sup> window range.

**Results**

Validation results showed that the proposed method was able to register CT lung datasets with TRE and ICE values <3 mm. In addition, the average number of voxel that failed the Gamma criteria was <3 %, which supports the clinical applicability of the propose registration mechanism.

**Conclusions**

The proposed 4D-CT registration computes the volumetric lung deformations within clinically viable accuracy.
