---
layout: publication
title: Estimation and Validation of Patient-Specific High-Resolution Lung Elasticity Derived from 4DCT
authors: Katelyn Hasse, Dylan O'Connell, Yugang Min, Jack Neylon, Daniel A. Low, Anand Santhanam
journal: Medical Physics, Volume 45, Issue 2
published: 2017-11-24
doi: https://doi.org/10.1002/mp.12697
link: https://aapm.onlinelibrary.wiley.com/doi/full/10.1002/mp.12697
---
**Purpose**

Lung diseases are commonly associated with changes in lung tissue's biomechanical properties. Functional imaging techniques, such as elastography, have shown great promise in measuring tissue's biomechanical properties, which could expand the utility and effectiveness of radiotherapy treatment planning. We present a novel methodology for characterizing a key biomechanical property, parenchymal elasticity, derived solely from 4DCT datasets.

**Methods**

Specifically, end‐inhalation and end‐exhalation breathing phases of the 4DCT datasets were deformably registered and the resulting displacement maps were considered to be ground‐truth. A mid‐exhalation image was also prepared for verification purposes. A GPU‐based biomechanical model was then generated from the patient end‐exhalation dataset and used as a forward model to iteratively solve for the elasticity distribution. Displacements at the surface of the lungs were applied as boundary constraints for the model‐guided tissue elastography, while the inner voxels were allowed to deform according to the linear elastic forces within the biomechanical model. A convergence criteria of 10% maximum deformation was employed for the iterative process.

**Results**

The lung tissue elasticity estimation was documented for a set of 15 4DCT patient datasets. Maximum lung deformations were observed to be between 6 and 31 mm. Our results showed that, on average, 89.91 ± 4.85% convergence was observed. A validation study consisting of mid‐exhalation breathing phases illustrated an accuracy of 87.13 ± 10.62%. Structural similarity, normalized cross‐correlation, and mutual information were used to quantify the degree of similarity between the following image pairs: (a) the model‐generated end‐exhalation and ground‐truth end‐exhalation, and (b) model‐generated mid‐exhalation images and ground‐truth mid‐exhalation.

**Conclusions**

Overall, the results suggest that the lung elasticity can be measured with approximately 90% convergence using routinely acquired clinical 4DCT scans, indicating the potential for a lung elastography implementation within the radiotherapy clinical workflow. The regional lung elasticity found here can lead to improved tissue sparing radiotherapy treatment plans, and more precise monitoring of treatment response.
