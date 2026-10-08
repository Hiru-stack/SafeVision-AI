
# SafeVision AI — Helmet Safety Detection System

SafeVision AI is an AI-powered helmet safety detection system developed using YOLO11.  
The system detects whether a person is wearing a helmet or not from an uploaded image.

The model was trained on a custom helmet dataset and deployed for browser-based image detection using ONNX Runtime Web.

## Project Overview

This project was created to demonstrate practical Computer Vision and object detection using YOLO.

The system can detect two classes:

- With Helmet
- Without Helmet

It can be used as a simple safety-monitoring solution for environments such as roads, construction sites, workplaces, and industrial areas.

## Model Performance

The trained YOLO11 model achieved:

- mAP@50: **81.3%**
- mAP@50-95: **49.7%**
- Precision: **76.8%**
- Recall: **80.7%**

Class-level mAP@50:

- Without Helmet: **76.5%**
- With Helmet: **86.1%**

## Technologies Used

- Python
- YOLO11
- Ultralytics
- PyTorch
- Computer Vision
- XML Annotation Processing
- ONNX
- ONNX Runtime Web
- HTML
- CSS
- JavaScript
- Google Colab
- GitHub Pages

## Dataset

The project uses a helmet detection dataset containing **764 annotated images**.

The original annotations were provided in Pascal VOC XML format.

As part of the project, the XML annotations were converted into YOLO format before training.

The dataset was divided into:

- 80% Training Data
- 20% Validation Data

The final converted dataset contained approximately:

- 611 training images
- 153 validation images

## Project Workflow

```text
Helmet Dataset
      ↓
XML Annotations
      ↓
XML to YOLO Conversion
      ↓
Training / Validation Split
      ↓
YOLO11 Model Training
      ↓
Model Evaluation
      ↓
best.pt
      ↓
ONNX Export
      ↓
best.onnx
      ↓
Browser-Based Detection
      ↓
SafeVision AI Web Interface

- Hirusha Jayasundara
