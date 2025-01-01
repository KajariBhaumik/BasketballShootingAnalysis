# Basketball Shooting Analysis with Computer Vision

This project leverages computer vision to automate basketball shot analysis, focusing on detecting key frames like the release frame and identifying critical objects. The goal is to provide actionable insights to enhance player performance and coaching strategies.

## Highlights
- <b> Object Detection:</b> Fine-tuned YOLOv8 to detect basketball, shooter, and hands with high precision and recall.
- <b> Release Frame Detection:</b> Automated identification of the frame where the ball is released using a custom-trained YOLO class.
- <b> Tools Used:</b> OpenCV for video processing, Roboflow for annotation, and Google Colab Pro for development.

## Data Pipeline
<b> 1. Data Collection:</b> Extracted frames (10th frame) from short videos (3–4 seconds, 60–100 fps).
<b> Annotation & Augmentation:</b> Annotated frames using Roboflow and enhanced dataset diversity with flipping and scaling.
<b> Training:</b> Fine-tuned YOLOv8-small model with 50 epochs, AdamW optimizer, and resized frames (640x640).

## Results
<b> Detection Accuracy:</b> >95% precision and recall across classes (basketball, shooter, hand, net).
</b> Model Metrics:</b> Precision-Recall curve highlights the YOLOv8 model’s reliability.
<details> <summary>Model Performance</summary> <p align="center"> <img src="path/to/precision_recall_curve.png" alt="Precision-Recall Curve" width="400"/> </p> </details>

## Tools and Libraries
Libraries: OpenCV, Roboflow, YOLOv8 by Ultralytics.
Platform: Developed and tested on Google Colab Pro.
