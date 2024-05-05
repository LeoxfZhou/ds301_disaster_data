# Classify the Type of Natural Disaster Based on Post-Event Building Images

Group members: Leo Zhou, Ashley Tsao, Denise Chow

All data and checkpoint models used in this project can be accessed here: https://drive.google.com/drive/folders/1-JIpjx58x5l_XO4wCzrtfmqSY9q3hhSY?usp=sharing

## Project Description

As the frequency and intensity of natural disasters continue to rise globally, the ability to quickly and accurately identify the type of disaster that has impacted a building becomes increasingly important. 
Classifying the type of natural disaster based on the impact on buildings is crucial for several reasons: it enables targeted structural assessments and repairs, informs the updating of building codes and safety regulations, streamlines insurance processing, aids in urban planning and resilience building, and enriches historical data for improved predictive modeling.
Understanding whether a structure has been affected by flooding, hurricanes, fires, or earthquakes helps tailor the recovery efforts and preventive measures specific to the nature of the damage.

This project aims to develop a tool that uses machine learning to analyze images of buildings post-disaster and classify the type of natural disaster that the structures have endured.
By leveraging advanced image recognition and artificial intelligence techniques, the tool will provide vital information that enhances disaster response, aids in reconstruction, and ultimately contributes to safer and more resilient communities.

We developed an initial baseline CNN model and subsequently, we explored three distinct hyperparameter optimization strategies: Random Search, Bayesian Search, and Hyperband. 
These methods were applied to our validation set to identify the model configuration that yields the highest accuracy. 
We also implemented transfer learning to enhance model performance further and use ResNet-18 as the teacher model.
Within this framework, we incorporated additional transformation augmentations, utilized distillation loss, and implemented a learning rate schedule.
Moreover, we constructed a more sophisticated and complex CNN model featuring weighted loss functions and increased regularization to improve robustness and accuracy.
The more complex CNN model class defines a custom convolutional neural network architecture tailored for disaster type classification from post-disaster images.
It uses multiple layers which are designed to extract hierarchical features from input images, as well as dropout layers and RELU functions to better generate class probabilities.

## Data

The datasets were from Maxar’s Open Data Program, consisting of building damage imagery for six different types of disasters and fifteen countries. 
Link to dataset: https://xview2.org/

## Project Structure 

This repository contains various google colab notebooks.
Each notebook contains code for both datasets and transfer learning.

