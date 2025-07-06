# Helmet Detection
---
## About the project<br/>
This project implements a helmet detection system using the YOLO (You Only Look Once) object detection models, primarily YOLOv11 and YOLOv12. It is designed to identify whether a person is wearing a helmet in real-time video streams or images. This kind of system is especially useful for monitoring safety compliance on construction sites, industrial zones, or roadways.

**YOLO model, Object Detection, Pytorch, Two-wheeler, Data annotation, Ultralytics, Machine learning**<br/>

**Data collection and preprocessing**<br/>
Dataset Information:<br/>
- The dataset includes **1756 images**
- No of classes: **2**  
- class_names: **['helmet', 'without helmet']**

**Data annotation**<br/>
- The dataset is annotated and preprocessed using Roboflow 
- Objects are annotated in YOLOv11 and YOLOv12 format.
  The following pre-processing was applied to each image:
  * Auto-orientation of pixel data (with EXIF-orientation stripping)
  * Resize to 640x640 (Stretch)
  The following augmentation was applied to create 3 versions of each source image:
  * 50% probability of horizontal flip
  * 50% probability of vertical flip
  * Equal probability of one of the following 90-degree rotations: none, clockwise, counter-clockwise, upside-down
  * Random rotation of between -15 and +15 degrees
  * Salt and pepper noise was applied to 0.1 percent of pixels

## Setup and installation
---
**Dependencies for the project**<br/>
- torch = 2.6.0+cu126
- roboflow = 1.1.54 
- python = 3.13.2
- numpy = 2.1.1
- matplotlib = 3.10.0
- ultralytics = 8.3.96
- pandas = 2.2.3 <br/>

**Steps for running the project**
1. **Run the jupyter notebook**<br/> 
   **For Yolov11**<br/>
   jupyter notebook Helmet_detection_yolov11-github.ipynb<br/>
   **For Yolov12**<br/>
   jupyter notebook Helmet_detection_yolov12-github.ipynb<br/>
   
## Results
---
**Yolov11**<br/>
<img src="https://raw.githubusercontent.com/syssoni/Helmet_detection/main/Results/confusion_matrix_normalized.png" alt="Confusion Matrix Normalised v11" width="70%">
<img src="https://raw.githubusercontent.com/syssoni/Helmet_detection/main/Results/PR_curve.png" alt="PR curve v11" width="70%"><br/><br/>

**Yolov12**<br/>
<img src="https://raw.githubusercontent.com/syssoni/Helmet_detection/main/Results/confusion_matrix_normalized_v12.png" alt="Confusion Matrix Normalised v12" width="70%">
<img src="https://raw.githubusercontent.com/syssoni/Helmet_detection/main/Results/PR_curve_v12.png" alt="PR curve v12" width="70%"><br/>

**Project Open for suggestions and changes and use**


