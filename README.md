# MoveMate's Pose Classifier Machine Learning Model
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Table of Contents
- [Description](#description)
- [Architecture](#architecture)
- [Results](#results)
- [Dependencies](#dependencies)
- [File Structure](#file-structure)

## Description
This model leverages the MoveNet model, a lightweight machine learning model for pose estimation, and TensorFlow Lite, a framework for running machine learning models on edge devices. This model showcases how to perform real-time pose estimation and classification, making it suitable for applications such as fitness tracking, gesture recognition, and more. In this case, we developed two models to classify Push Up and Sit Up poses. Our model can be fed with data from other poses and be used to classify other poses as needed.

## Architecture
![pose_classifier tflite](https://github.com/pdshi/activity-recognition-model/assets/85791158/979760dd-8912-4d55-8272-55ffe4aaeb32)

## Results
Inference Results Using Movenet Thunder
![negative-push-up_jpg rf 18c61504c4970e02cb09247d2f0b3538](https://github.com/pdshi/activity-recognition-model/assets/85791158/47f3ea96-285a-4418-9f35-a0191d01aeb9)
![health-push-up-1140x600_png rf e75e5b15437053d951a34a74d28637c0](https://github.com/pdshi/activity-recognition-model/assets/85791158/3efa6e56-f324-4cef-a157-e083e12cc39d)
![Screenshot 2023-06-10 133400](https://github.com/pdshi/activity-recognition-model/assets/85791158/730f87fc-3c66-4f0d-83b0-519ac8c31126)
![Screenshot 2023-06-07 191842](https://github.com/pdshi/activity-recognition-model/assets/85791158/a1c297bd-42a6-4239-9cdc-8e2edaa76665)

Sit Up Classifier Train Result 
![image](https://github.com/pdshi/activity-recognition-model/assets/85791158/51655d58-e985-46d9-a679-0a69907b4f51)
![image](https://github.com/pdshi/activity-recognition-model/assets/85791158/6405f098-3dfa-4406-aafa-87e494f219a9)

Push Up Classifier Train Result
![image](https://github.com/pdshi/activity-recognition-model/assets/85791158/b0a6792c-a12b-40cd-a87e-078136867209)
![image](https://github.com/pdshi/activity-recognition-model/assets/85791158/7e537d9b-31e9-4e5e-a120-5bf07fd72b74)

The final accuracy after exporting the models into TFLite are as follows:
- Accuracy of Push Up TFLite model: 1.0
- Accuracy of Sit Up TFLite model: 0.9807692307692307

## Dependencies
Here are the dependencies and libraries needed to run the notebook
- Python
- TensorFlow and TensorFlow Hub
- OpenCV
- Numpy
- Pandas
- Matplotlib
- Scikit-learn

## File Structure
- `Push Up Model`: Directory containing the notebook and outputs for Push Up Classification.
- `Sit Up Model`: Directory containing the notebook and outputs for Sit Up Classification.
- `Supporting Programs`: Directory containing the supporting programs to compress and augment the dataset.

Push Up Model and Sit Up Model directory consists of:
- Notebook for the machine learning model
- Base MoveNet Thunder model for pose estimation
- Output classification model in tflite format
- Labels for the classes
- CSV of preprocessed data
- Saved best weights

The dataset used for the models can be found here
Push Up Dataset: https://drive.google.com/drive/folders/1DmlWEiONg682cgAhCEg5U3__oE8Wng4i?usp=sharing
Sit Up Dataset: https://drive.google.com/drive/folders/1qcyGe0QFFDivjcH310Yqgcq72tnsAYrR?usp=sharing
