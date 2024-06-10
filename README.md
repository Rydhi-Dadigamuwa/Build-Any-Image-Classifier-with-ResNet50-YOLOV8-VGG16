# Build Any Image Classifier
<br/>

This repository contains three notebooks for building image classifiers by using VGG16, ResNet50 and YOLOV8
<br/>
<br/>



## 1. VGG16 Architecture

![VGG16 Architecture](VGG16.png)

The above image shows the VGG16 architecture. "Image_Classifier_using_VGG16.ipynb" notebook shows,
### Part 1: Building an Image Classifier from Scratch
First half of the notebook provide a guide to build image classifier using VGG16 from scratch. But you can see, its loss is greater than the accuracy. This is because VGG16 is a complex architecture. In order to get higher accuracy 
we need to train under more epochs or increase the dataset

### Part 2: Improving Accuracy with Pretrained VGG16 Model
As a solution for that, then import VGG16 model from tensorflow with "ImageNet" weights. This increases the model accuracy.

<br/>

## 2. ResNet50
ResNet50 is a deep learning model introduced by Microsoft Research in 2015 for visual recognition. The name “ResNet” stands for “Residual Networks,” and the “50” indicates that the model has 50 layers. 
This provide greter accuracy than VGG16 model.

<br/>


## 3. YOLOV8
YOLOv8 is the latest iteration in the YOLO series developed by Ultralytics. In this notebook, provide a guide to use YOLOV8 for image classification. The main advatage of this is that, this is very easy to build.
It is only need to upload the dataset folder which contain train, validation and test dataset folders and provide the dataset folder path to the results = model.train(data=dataset_path, epochs=20) function.
It will automatically identify classes in our dataset by reading the folder name. 
<br/>

As an  example, in this notebook, fruits and vegetables are classified into 36 categories. The dataset is organized such that the train, validation, and test directories each contain 36 subdirectories, with each subdirectory named after a specific class
and containing corresponding images.

<br/>
In addition to that, YOLOV8 provide higher accuracy than VGG16.


<br/>
To use YOLOV8 in local machine please install following dependancies using following command
<br/>
<br/>


```
pip install torch
```
```
pip install ultralytics
```

# Notes:
1. Replace train, validation and test data paths with the actual paths to your training and validation datasets.
2. Replace test example path (image path) with the actual paths to your image.
<br/>

# Dataset
Dataset is obtained from keggale platform.
