# Battery Health Prediction using Deep Hybrid Learning

This repository contains the code and data for the research paper "Battery Health Prediction using Deep Hybrid Learning" by Rahul Anil Nair, Dev Karan Suresh, and Rajeswari D.

## Abstract

The research focuses on the impact of various factors on the battery life of electric vehicles (EVs). The paper examines the effects of road conditions on battery life and categorizes routes based on the number of brakes applied upon arrival at the destination. The aim is to develop recommendations for drivers on how to optimize their driving habits to extend the battery's lifespan. The research uses Deep Hybrid Learning to integrate three pre-trained models, VGG16, Resnet50, and VGG19, with two boosting algorithms: XGBoost and AdaBoost.

## Dataset

The original dataset includes an EV's latitude, longitude, Battery SOC, Air Conditioning Power, Heater Power, Battery Voltage, Battery Current, and Vehicle Speed from start to finish. The dataset was used to generate satellite images of the vehicle paths using Google Earth. These images were then categorized into 'best' and 'worst' routes based on the number of brakes applied upon arrival at the destination.

## Preprocessing

The original dataset was preprocessed in phases. First, the electric cars' vehicle ids were obtained, and the routes of these vehicles were split and stored in new data frames that were further segregated based on the route id. These data frames were inserted into Google Earth Pro where satellite images of the routes were obtained. These were then segregated into best and worst images based on the number of brakes applied throughout the journey.

## Models

Six deep hybrid learning models were made to analyze how accurately the category of the given routes can be predicted. Deep hybrid learning models involve combining a pre-trained model with a boosting algorithm like XGBoost or AdaBoost to enhance the accuracy of the predictions and reduce overfitting or underfitting. The pre-trained models used for this purpose are as follows: VGG16, Resnet50, and VGG19. Each of these pre-trained models are combined with XGBoost and AdaBoost and the results are represented by a confusion matrix.

## Usage

To run the code, follow these steps:

1. Clone the repository.
2. Install the necessary dependencies.
3. Download the files for images which will be given in this readme file.
4. Run the model training scripts after changing the paths of the images as per your needs.

## Dependencies

- Python 3.8+
- Keras
- TensorFlow
- XGBoost
- AdaBoost
- Google Earth Pro

## Google Drive Link for Images
-Best route Images:-https://drive.google.com/drive/folders/1w_48ZhSkBVcWSvisdE38B5oVOvIT-SHW?usp=sharing
-Worst route Images:-https://drive.google.com/drive/folders/1JzS18-bX30dxajRYXQDaCfbvC45Sc9kW?usp=sharing
-Augmented Images:- https://drive.google.com/drive/folders/1DosW-ZSkZOcxKA9idoeuDVOB01Axjm4n?usp=sharing
-Other files:- https://drive.google.com/drive/folders/1-nK8unWyKawJsMt1CK-WNQ0OI8umgW3E?usp=sharing

## Contact

For any queries, please contact:

- Rahul Anil Nair: rahulanilnair1220@gmail.com
- Dev Karan Suresh: devkaran7501@gmail.com
- Rajeswari D (Corresponding author): drajiit@gmail.com

## License

This project is licensed under the MIT License.
