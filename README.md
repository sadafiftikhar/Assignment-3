# Assignment 3

Image Classification using CNN

## Dataset
Intel-Classification-Images
The dataset is divided into 3 categories i.e. training set, validation set, and test set.
Import data from Kaggle

## Model Setting
Epochs = 10
```python
modelx = Flatten()(base_model.output)
modelx = Dense(1024, activation='relu')(modelx)
modelx = Dense(256, activation='relu')(modelx)
# modelx = Dense(256, activation='relu')(modelx)
model = Dense(len(folders), activation='softmax')(modelx)
```

## Model Summary
![alt text](https://github.com/sadafiftikhar/Assignment-3/blob/main/images/summary.PNG?raw=true)

## Trained Model Weights 
https://drive.google.com/file/d/1-1xq-BqAficdpdfwRov2gyKx5MBmZ0Rx/view?usp=sharing

## Results
**Accuracy**
Training_accuracy: 88.80%
validation_accuracy: 84.9%
<br />
![alt text](https://github.com/sadafiftikhar/Assignment-3/blob/main/images/acc_graph.png?raw=true)

**Loss**
Training_loss: 30.61% 
validation_loss: 52.05%
<br />
![alt text](https://github.com/sadafiftikhar/Assignment-3/blob/main/images/loss_graph.png?raw=true)

**Confusion Matrix**
<br />
![alt text](https://github.com/sadafiftikhar/Assignment-3/blob/main/images/confusion_matrix.png?raw=true)
