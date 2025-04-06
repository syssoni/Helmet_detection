# Helmet_detection
The project focuses on detecting helmets on two wheelers 
The models used are : yolov11n and yolov12n models are used

The dataset is annotated and preprocessed using roboflow 
The information for dataset is given below:

The dataset includes 1756 images
no of classes: 2  
class_names: ['helmet', 'without helmet']
Objects are annotated in YOLOv11 and YOLOv12 format.

The following pre-processing was applied to each image:
* Auto-orientation of pixel data (with EXIF-orientation stripping)
* Resize to 640x640 (Stretch)

The following augmentation was applied to create 3 versions of each source image:
* 50% probability of horizontal flip
* 50% probability of vertical flip
* Equal probability of one of the following 90-degree rotations: none, clockwise, counter-clockwise, upside-down
* Random rotation of between -15 and +15 degrees
* Salt and pepper noise was applied to 0.1 percent of pixels
