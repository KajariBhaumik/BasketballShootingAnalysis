# Basketball Shot Analysis with Computer Vision

This project leverages computer vision to automate basketball shot analysis, focusing on detecting key frames like the release frame and identifying critical objects. The goal is to provide actionable insights to enhance player performance and coaching strategies.

## Highlights
- **Object Detection:** Fine-tuned YOLOv8 to detect basketball, shooter, and hands with high precision and recall.
- **Release Frame Detection:** Automated identification of the frame where the ball is released using a custom-trained YOLO class.
- **Tools Used:** OpenCV for video processing, Roboflow for annotation, and Google Colab Pro for development.

## Data Pipeline
1. **Data Collection:** Extracted frames (10th frame) from short videos (3–4 seconds, 60–100 fps).
2. **Annotation & Augmentation:** Annotated frames using [Roboflow](https://roboflow.com) and enhanced dataset diversity with flipping and scaling.
3. **Training:** Fine-tuned YOLOv8-small model with 50 epochs, AdamW optimizer, and resized frames (640x640).

### Sample Frames
<details>
<summary>Click to view examples of annotated and augmented frames</summary>
<p align="center">
<img src="path/to/annotation_example.png" alt="Annotated Frame" width="400"/>
<br>**Figure:** Annotated frame highlighting basketball, shooter, and hand.
<br><br>
<img src="path/to/augmented_frame.png" alt="Augmented Frame" width="400"/>
<br>**Figure:** Augmented frame after flipping and scaling for model robustness.
</p>
</details>

---

## Results
- **Detection Accuracy:** >95% precision and recall across classes (basketball, shooter, hand, net).
- **Model Metrics:** Precision-Recall curve highlights the YOLOv8 model’s reliability.

### Model Performance
<details>
<summary>Click to view Precision-Recall curve</summary>
<p align="center">
<img src="path/to/precision_recall_curve.png" alt="Precision-Recall Curve" width="400"/>
<br>**Figure:** Precision-Recall curve showcasing model performance across classes.
</p>
</details>

---

## Tools and Libraries
- **Libraries:** OpenCV, Roboflow, YOLOv8 by Ultralytics.
- **Platform:** Developed and tested on Google Colab Pro.

## Acknowledgements
This project was completed under the mentorship of [Coach Dave Love](https://www.instagram.com/coachdavelove/?hl=en) at CDL Basketball Enterprises, with support from Dr. Robert Fox and Roboflow.
