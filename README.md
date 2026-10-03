# YOLO Helmet Detection

## Overview

A Computer Vision object detection project built using YOLO to detect:

- Helmet
- Head
- Person

The project demonstrates the complete object detection pipeline, from dataset preparation and annotation conversion to model training and evaluation.

## Dataset

The project uses the Hard Hat Workers dataset from Kaggle.

- Total images: 5,000
- Total annotations: 5,000
- Original annotation format: Pascal VOC (XML)

## Dataset Preparation

The original Pascal VOC annotations were converted into YOLO format.

Class mapping:

- 0 → Helmet
- 1 → Head
- 2 → Person

The dataset was split into:

- Training: 3,500 images
- Validation: 1,000 images
- Testing: 500 images

## Model Training

The model was trained using the Ultralytics YOLO framework on Google Colab with GPU acceleration.

The training pipeline includes:

- Dataset loading
- Annotation parsing
- Pascal VOC to YOLO conversion
- Train / Validation / Test splitting
- Dataset configuration
- YOLO model training
- Model evaluation
- Object detection inference

## Dataset Analysis

The dataset contains a class imbalance, especially for the Person class.

Person bounding boxes:

- Total: 498
- Small: 60
- Medium: 327
- Large: 111

This analysis was performed to better understand the dataset before improving the model using techniques such as data augmentation or oversampling.

## Technologies

- Python
- YOLO
- Ultralytics
- Computer Vision
- Google Colab
- Kaggle
- Pascal VOC
- OpenCV

## Project Goal

The goal of this project is to build an object detection system capable of identifying helmets, uncovered heads, and people in workplace environments.

This type of system can be used as a foundation for automated workplace safety monitoring.

## Notebook

The complete implementation, dataset preparation, training pipeline, and experiments are available in:

`YOLO_Helmet_Detection.ipynb`
