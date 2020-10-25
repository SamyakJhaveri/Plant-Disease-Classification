
# Plant Species and Disease Classification 
## Introduction
Early and accurate detection and diagnosis of plant disease are key factors in plant production and the reduction of both qualitative and quantitative losses in crop yield. 

Non-destructive, sensor-based methods support and expand upon and/or molecular approaches to plant disease assessment. The most relevant application of sensor-based analyses  are precision agriculture and plant phenotyping.

Computer vision and machine-learning solutions offer great opportunities for the automatic recognition of sick plants by visual inspection of damaged leaves.

An automatic plant-disease detection system provides clear benefit in monitoring of large fields, as this is the only approach that provides a chance to discover diseases at an early stage. The computer vision core system inspects image flow from cameras, detects diseased leaves, and performs classification. The inspection results can be provided in various ways.

We’ve attempted to build a classifier system using Google’s TensorFlow API to train multiple model architectures on a readily available plant leaf dataset provided by Kaggle. 

Once trained, these model architectures are tested using previously unseen data (unseen by the training algorithm) to make classifications from the labelled data they were trained on. Parameters such as confidence and accuracy of classification are the ones that are optimized and used as rubrics of assessment. 

One of the most important characteristics of this project is that it uses a concept called transfer learning to train the models which makes the entire process much faster with very little loss in efficiency/accuracy.

## Transfer Learning
Transfer learning generally refers to a process where a model trained on one problem is used in some way on a second related problem.<br>

In deep learning, transfer learning is a technique whereby a neural network model is first trained on a problem similar to the problem that is being solved. 
One or more layers from the trained model are then used in a new model trained on the problem of interest.

![Transfer Learning](images/pdc%202.png)
Transfer learning has the benefit of decreasing the training time for a neural network model and can result in lower generalization error.<br>

The weights in re-used layers may be used as the starting point for the training process and adapted in response to the new problem. This usage treats transfer learning as a type of weight initialization scheme. This may be useful when the first related problem has a lot more labeled data than the problem of interest and the similarity in the structure of the problem may be useful in both contexts. The objective is to take advantage of data from the first setting to extract information that may be useful when learning or even when directly making predictions in the second setting.

![Transfer Learning vs Traditional Machine Learning](images/pdc%201.png)
A range of high-performing models have been developed for image classification and demonstrated on the annual ImageNet Large Scale Visual Recognition Challenge, or ILSVRC.<br>

This challenge, often referred to simply as ImageNet, given the source of the image used in the competition, has resulted in a number of innovations in the architecture and training of convolutional neural networks. In addition, many of the models used in the competitions have been released under a permissive license.<br>
These models can be used as the basis for transfer learning in computer vision applications.

## Conclusion
With the help of transfer learning and Google Colab’s GPUs, this project successfully achieves a high accuracy rate at classifying the plant species and diseases without compromising speed at which the models can be trained or tested. <br>
![Training vs Testing Accuracy](images/pdc%203.png)
![Testing 1](images/pdc%204.png)
![Testing 2](images/pdc%205.png)
![Testing 3](images/pdc%206.png)


## Societal Applications
This project highlights the usefulness of two main applications:<br><br>
1)	The use of computer vision and machine learning in detecting and diagnosing plant species and diseases that can make systems such as precision farming and 
plant phenotyping possible.<br>
2)	The versatility of transfer learning, especially in image-based classification models that can be easily maneuvered to work for a wide range of applications 
besides on vegetation.
