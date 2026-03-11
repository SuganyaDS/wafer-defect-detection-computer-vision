# Semiconductor Wafer Defect Detection using Computer Vision

This project develops a classical computer vision pipeline for detecting and classifying semiconductor wafer defect patterns using machine learning.

## Problem
Wafer inspection is critical in semiconductor manufacturing. Detecting defect patterns such as Center, Donut, Edge-Ring, and Scratch helps improve yield and manufacturing quality.

## Dataset
A subset of the WM-811K wafer map dataset was used. Each wafer map represents chip states across the wafer.

Pixel values:
0 – outside wafer  
1 – normal chip  
2 – defective chip  

## Methodology

Wafer Map
→ Gaussian Filtering
→ Edge Detection (Canny)
→ Morphological Processing
→ Feature Extraction (HOG)
→ SVM Classification

## Results

The SVM classifier achieved approximately **85% accuracy** on wafer defect classification.

The model performs particularly well for Edge-Ring defects while Donut and Scratch defects are more challenging.

## Visualization

The project also includes **defect localization**, where contour detection highlights defect regions within wafer maps.

## Technologies Used

Python  
OpenCV  
Scikit-learn  
Scikit-image  
Matplotlib  

## Applications

This approach demonstrates how computer vision algorithms can be used in **automated semiconductor inspection systems**.
