# Assignment 51
# Hello Deep learning

# Face Recognition

 + I have implemented a model in this repository which an recognize the Iranian celebrities (which are in used dataset) by receiving photos of their faces.


+ In this session I use a deepface library for face recognition. 

+ Deepface is a library that use for extracting feature of human faces. 
This library used different deep learning algorithms for its purpose.


## How to Install
Run following commend :
```
pip install -r requirments.txt
```

## How to Run
```
Run Face_Recognition.ipynb file in jupyter notebook
```


## Description

I've done some step to achieve end goal.

1. At first I write a function to use a dataset which include picture of different persons to produce features and labels.

   When all features are extracted, I stored them in ```persian_faces.csv``` file in dataset folder. I wrote a function which name is `generate_dataset` for this part. 

2. Then I preprocess data and onehot the labels. labels are the names of that persons that exist in the dataset.

3. And then I made a model with tensorflow to train the features with labels.

4. Finally I use sample pictures to predict person.

  My model can achieve 98% accuracy for train data and 82% accuracy for test data. Finally I stored my trained model in weights folder and named it ```PersianFaces.keras``` .
 

 ## **Result**

### Train
<img src="Output\Train.png">


### Loss and Accuracy

|          | Accuracy | Loss
| -------- | -------- | ---
Train      | 0.9534   | 0.0466
Validation |  0.7968    | 0.2032







