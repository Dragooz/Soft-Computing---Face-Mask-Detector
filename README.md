# Soft-Computing: Face Mask Detection

## Face Mask Detection Project
COVID-19 pandamic is now greatly influences the life-style of humans. Everyone that going out to the public should wear mask to protect themselves as well as other people. This project focus mainly on creating a model that is able to classify whether the people wear a mask correctly, incorrectly or do not wear mask so that action can be taken on those who do not wear a mask properly. The model will be deployed associated with face detector model, with the aid of OpenCV.

### Objectives: 
1. To detect whether the person wear a mask correctly, wear a mask incorrectly or do not wear a mask.
2. To evaluate the confidence of the model on the detection of mask.

### Data Sources:
1. https://github.com/cabani/MaskedFace-Net 
(correct_mask:
https://esigelec-my.sharepoint.com/personal/cabani_esigelec_fr/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fcabani%5Fesigelec%5Ffr%2FDocuments%2FMaskedFaceNetDataset%2FCMFD&originalPath=aHR0cHM6Ly9lc2lnZWxlYy1teS5zaGFyZXBvaW50LmNvbS86ZjovZy9wZXJzb25hbC9jYWJhbmlfZXNpZ2VsZWNfZnIvRXYzR2RuUVN5enhQanl6VTVFbEhxYWdCbGtSQ2FLbm5DSTg1aVgtZDFMNE9IQT9ydGltZT10SFpaaHdBcDJVZw )
(incorrect_mask:
https://esigelec-my.sharepoint.com/personal/cabani_esigelec_fr/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fcabani%5Fesigelec%5Ffr%2FDocuments%2FMaskedFaceNetDataset%2FIMFD&originalPath=aHR0cHM6Ly9lc2lnZWxlYy1teS5zaGFyZXBvaW50LmNvbS86ZjovZy9wZXJzb25hbC9jYWJhbmlfZXNpZ2VsZWNfZnIvRWlyalM4ZXc3LTVMbk84STU2VWs2M3dCS2Vid1NsdWtGQkZCYU84TjI1d24zZz9ydGltZT1vYllJcWdBcDJVZw )

3. https://www.kaggle.com/omkargurav/face-mask-dataset (without_mask)

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

## Instruction to use the notebook

1. Modify variables by searching 'modify here' in the notebook according to your preferences.
2. Install all the requirements needed as mentioned in the notebook.
3. Enjoy!





