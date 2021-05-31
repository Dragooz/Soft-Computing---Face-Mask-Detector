# Soft-Computing---Face-Mask-Detector

## Face Mask Detector Project
To detect whether a person wear the mask correctly, incorrectly or do not wear a mask

### Objectives: 
1. To detect whether the person wear a mask correctly, wear a mask incorrectly or do not wear a mask.
2. To evaluate the confidence of the model on the detection of mask.

### Data Sources:
1. https://github.com/cabani/MaskedFace-Net (correct_mask, incorrect_mask)
2. https://www.kaggle.com/omkargurav/face-mask-dataset (without_mask)

### Codes Referred:
1. https://www.pyimagesearch.com/2020/05/04/covid-19-face-mask-detector-with-opencv-keras-tensorflow-and-deep-learning/

## About the notebook

### It have mainly 2 parts:
#### Train model to classify among wearing mask correctly, incorrectly or not wearing a mask
1. MobileNetV2 is used as a base model.
2. 1000 images from each class are used to train the model.
3. Result of the training: <br>
![plot](https://user-images.githubusercontent.com/47239545/120218868-ef2ea480-c26c-11eb-9516-3182c9ef794d.png)

#### Deploying mask detector by associating with face detector model (Caffe model)
1. Input an image with people
2. Output an image with the a square boundary, associated with labels and a square boundary (green for correctly wearing mask, red for incorrectly wearing mask or do not wear mask)

### Sample input/output image
#### Input:
![the-rock](https://user-images.githubusercontent.com/47239545/120218796-d7572080-c26c-11eb-9ee4-8c74b7917c8d.jpg)

#### Output:
![the-rock_checked](https://user-images.githubusercontent.com/47239545/120218794-d58d5d00-c26c-11eb-97fc-c1680d4b1a99.jpg)





