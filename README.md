# Advanced Computer Vision: Night-Time Lights Analysis
**Course:** A1303 - Computer Vision (Spring 2026)  
**Instructor:** Ms. Hina Rashid  
**Students:** M Awais (231180) & M Zain (231194)  
**Group:** 11  

## 🌌 Project Overview
This repository contains a full end-to-end Computer Vision pipeline applied to the **Night-Time Lights of the World** dataset (Remote Sensing/GIS). The project transitions from raw satellite sensor data to high-level urban cluster identification.

## 🛠️ Implementation Phases

### Phase 1: Radiometric Pre-processing (Assignment 1)
* **Objective:** Mitigating sensor noise and atmospheric blooming in satellite data.
* **Bit-Depth ID:** Analysis of radiometric resolution to prevent **False Contouring**.
* **Filtering:** Implementation of Gaussian and Median filters to reduce sensor noise.
* **Metrics:** Quantified restoration using **PSNR** (Peak Signal-to-Noise Ratio).

### Phase 2: Structural Representation (Assignment 2)
* **Segmentation:** Isolating city light clusters using Otsu's Thresholding.
* **Geometry:** Implementation of the **Convex Hull** (Jarvis March algorithm) to map urban boundaries.
* **Chain Coding:** 8-directional chain coding for boundary tracking to ensure rotational invariance.

### Phase 3: Statistical Texture Analysis (Assignment 3)
* **Feature Extraction:** Gray-Level Co-occurrence Matrix (**GLCM**) calculation.
* **Descriptors:** Extraction of Energy, Entropy, and Contrast of light intensity.
* **Output:** A comprehensive feature vector CSV for urban vs. rural classification.

### Final Project: Deep Vision Pipeline
* **Model:** CNN/YOLO integration for automated light detection.
* **Evaluation:** Performance measured via Confusion Matrix and Precision/Recall analysis.

## 📂 Repository Structure
* **/Code**: `CV_Group11_Final.ipynb`
* **/Data**: Sample raw images and cleaned outputs.
* **/Output**: `Group11_Feature_Vectors.csv`
* **/Report**: 15-page Professional Research Paper (PDF).

## 🚀 Setup & Usage
1. Open the notebook in **Google Colab**.
2. Upload your `dataset_cv.zip` to the `/content/` directory.
3. Run all cells to generate the feature vectors and processed images.