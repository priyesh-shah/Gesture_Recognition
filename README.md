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
Model 14 (Final model) has good accuracy scores and less parameters compared to other models. Even though model 9 has a better accuracy scores there are considerably more parameters and hence Model 14 is chosen as the final model.

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
Created by [@chandamouli] and [@priyesh-shah] - feel free to contact us!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->