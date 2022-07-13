# Gesture recognition using deep learning
> To build a deep learning model which can accurately detect 5 different gestures.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- To develop a cool feature in the smart-tv that can recognise five different gestures performed by the user which will help users control the TV without using a remote. We will be using deep learning models to achieve this gesture recognition
- The training data consists of a few hundred videos categorised into one of the five classes. Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images). These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use.

- The data set contains the following data :

    * Thumbs up: Increase the volume
    * Thumbs down: Decrease the volume
    * Left swipe: 'Jump' backwards 10 seconds
    * Right swipe: 'Jump' forward 10 seconds
    * Stop: Pause the movie

The following models are created in this project
   1. Create a base conv3d model 
   2. Experiment and create multiple models to get a better accuracy
   3. Also experiment with different architectures like Time Distributed + ConvLSTM 2D 
   4. Choose the final model accuracy and number of parameters
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- From base model or model 1
    * The model is overfitting because the training accuracy is around 70% but validation accuracy is around 51% 
    * also after epoch 7, there is a huge deviation in the loss between validation and training.
- From model 1 post data augmentation
    * The overfitting issue from model1 is resolved due to data augmentation
    * However the training accuracy dropped from 70% to 40%
    * Number of epocs can be increased or more layers added and/or tune the hyper parameters to increase accuracy
- From model 2 post class re-balance
    * Accuracy on training data has increased by class rebalance using Augmentor library
    * Model is still overfitting
    * Overfitting can be resolved by adding more layers, neurons and dropout layers
    * Accuracy can be further improved by tuning the hyperparameters

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- numpy
- pandas
- tensorflow - Keras
- imageio
- google colab
- Jarvis


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- This project was inspired by deep learning models for gesture recognition assignment from upgrad
- Stackoverflow for certain code snippets and to understand the usage of augmentation
- tensorflow official documentation to understand various api's used in this project

## Team
 - Chandramouli krishnamurthy
 - Priyesh Shah (Moderator)

## Contact
Created by [@chandamouli] and [@priyeshah] - feel free to contact us!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->