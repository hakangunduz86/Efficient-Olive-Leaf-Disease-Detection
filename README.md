# Efficient-Olive-Leaf-Disease-Detection
 This repository provides the implementation of the preprocessing and feature extraction pipeline used in the study:  
 **Efficient Olive Leaf Disease Detection Using Deep Features, Composite Filter-Based Feature Selection, and Ensemble Learning**

## Dataset

The olive leaf disease images used in this study are obtained from the publicly available dataset:

**Olive Leaf Disease Dataset (Kaggle)**  
https://www.kaggle.com/datasets/serhathoca/zeytin
The dataset contains images of olive leaves belonging to two main categories:

- Healthy olive leaves
- Diseased olive leaves (Peacock Eye disease)

Images were captured under natural conditions and include variations in lighting, background, and leaf orientation.

### Dataset Download

To download the dataset:

1. Create a Kaggle account if you do not already have one.
2. Navigate to the dataset page:
   
   https://www.kaggle.com/datasets/serhathoca/zeytin

3. Download the dataset and extract it into your working directory.


## Overview

This project aims to develop an efficient and deployable olive leaf disease detection framework by:

- Removing background noise from field-acquired olive leaf images,
- Extracting deep features using pretrained convolutional neural networks,
- Supporting subsequent feature selection and ensemble learning stages.

The included Jupyter Notebook demonstrates the **image preprocessing and deep feature extraction pipeline** applied to representative olive leaf samples.

---

## Preprocessing Pipeline

The preprocessing workflow consists of the following steps:

1. Reading RGB olive leaf images
2. Color-based segmentation to isolate the leaf region
3. Morphological operations to refine segmentation masks
4. Background removal
5. Conversion to RGBA format with transparent background
6. Optional horizontal splitting of the leaf image
7. Deep feature extraction using pretrained CNN backbones

---

## Feature Extraction

- Pretrained CNN models used:
  - MobileNet
  - ResNet101
- Feature vectors are extracted from the final global pooling layers.
- Extracted features serve as input to filter-based feature selection and ensemble classification stages described in the manuscript.

---
---

## ⚙️ Requirements

The notebook was developed and tested using:

- Python 3.11
- TensorFlow
- NumPy
- OpenCV
- scikit-learn
- matplotlib

(Exact software versions and hardware details are reported in the manuscript.)

---

## Reproducibility Notes

This repository focuses on demonstrating the **preprocessing and feature extraction stages** of the proposed framework.

Feature selection strategies, classification models, ensemble learning methods, and evaluation protocols are fully described in the accompanying journal article.

---

## Citation

If you use this code, please cite:

> H. Gündüz et al., *Efficient Olive Leaf Disease Detection Using Deep Features, Composite Filter-Based Feature Selection, and Ensemble Learning*, 

---

## Contact

For questions or collaboration inquiries:

**Dr. Hakan Gündüz**  
Kocaeli University  
Department of Software Engineering
