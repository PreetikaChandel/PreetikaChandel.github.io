---
layout: post
title:  "Facial Expression Recognition"
date:   2016-05-15
categories: Machine-Learning

---

The human face reveals our current focus of attention,  affective state of the person, his temperament and personality; in brief, facial expressions regulate our interactions with the environment and people in our vicinity. Facial expression recognition is a visual pattern recognition problem. The issue of machine recognition of human facial expression includes three subproblem domains: (1) discovering faces in the scene, (2) extracting facial features from the detected face region, (3) analyzing the motional changes in the appearance of facial features, and classifying this information into some facial-expression-interpretative categories (e.g., emotions, facial muscle actions, etc.)

Presently, I am working on to create a facial expression recognizer to detect seven basic emotions (happy, sad, fear, anger, neutral, surprise, disgust). Having gone through various methods including PCA, SVM, Artificial Neural Network seemed most apt to be used as it significantly improves the accuracy and the robustness of local searching on faces with expression variation and ambiguous contours. 

As a part of this work, I had made use of Cohn Kanade database which currently includes 2105 digitized image sequences from 182 adult subjects of varying ethnicity, performing multiple tokens of most primary FACS action units. This involved the record of facial behavior of 210 adults between the ages of 18 and 50 years. The sample constituted 69% female, 31% male, 81% Euro-American, 13% Afro-American, and 6% other groups.

Here, neural network classifier takes gray scale image as input and gives an expression as output. This process is performed by first preprocessing the input image and then training or testing the image on  neural network which in turn classifies the image into one of the above mentioned categories of emotions. Steps involved are:

1. Training Neural Network with Input face images<br>
Back Propagation feed forward Artificial Neural Network is used for training the input face images. The computed Eigenfaces of the input face images are fed to the neural Networks. After setting the parameters of neural networks are trained with Eigenfaces of the input images via input layer, hidden layer and output layer. Each Eigenfaces image distance is compared with each other. The errors at the output layer are sent back to the previous layers that are hidden and weights are updated which minimize the error.

2. Testing the ANN with Tested Face Image<br>
For face recognition, the eigenfaces images of the test face image is intended by feature extraction based on PCA. This Eigenfaces image is given to the trained neural network. The tested Eigenfaces is compared with the Eigenfaces of the trained neural network for finest match result using the Log - sigmoid function values. The minimum distance between the tested Eigenfaces image and the trained input Eigenfaces image is not as much of as the threshold value. The maximum scored value corresponding to a particular expression depicts the likelihood of that expression of a person in an image.


__________________________________________________________________________________________________________________________________________________________


