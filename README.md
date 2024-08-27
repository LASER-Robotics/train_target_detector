# Train Target Detector

Welcome to the **Train Target Detector** project by the LASER Robotics team. This repository contains the implementation and training pipelines for detecting targets using computer vision techniques.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Training](#training)
  - [Dataset Preparation](#dataset-preparation)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Train Target Detector is designed to identify specific targets in images and video streams. The project utilizes deep learning models, primarily focusing on Convolutional Neural Networks (CNNs), to achieve accurate target detection.

## Features

- **Pre-trained Models**: Utilizes state-of-the-art pre-trained models like YOLO, SSD, and Faster R-CNN.
- **Custom Training**: Allows custom datasets for training the detector on specific target types.
- **Real-time Detection**: Capable of detecting targets in real-time from video feeds.
- **Multi-platform Support**: Compatible with both ROS and standalone Python scripts.
- **Visualization Tools**: Provides tools to visualize the detection results and model performance.

## Installation

To install the necessary dependencies, clone this repository and run the following commands:

``` 
git clone https://github.com/LASER-Robotics/train_target_detector.git
cd train_target_detector
pip install -r requirements.txt
```

Ensure you have Python 3.7+ and the necessary deep learning libraries like TensorFlow or PyTorch installed.

## Training

To initiate training, use the provided Jupyter Notebook:
```
train_target_detector/
    └───scripts/
        └───train-yolov8.ipynb
```
Open `train-yolov8.ipynb` in Jupyter Notebook to configure and run the training pipeline. This notebook allows you to set hyperparameters, specify datasets, and start the training process interactively.


### Dataset Preparation

Ensure your dataset is organized in the following structure:

```
dataset/
│
└───real/
    │
    └───train/
    │   └───images/
    │   └───annotations/
    │
    └───valid/
    |   └───images/
    |   └───annotations/
    │
    └───test/
        └───images/
        └───annotations/
```

- **train/images/**: Contains all training images.
- **train/annotations/**: Contains the corresponding annotations for the training images.
- **valid/images/**: Contains all validation images.
- **valid/annotations/**: Contains the corresponding annotations for the validation images.
- **test/images/**: Contains all test images.
- **test/annotations/**: Contains the corresponding annotations for the test images.
## Contributing

We welcome contributions from the community. If you encounter any bugs, have suggestions for improvements, or would like to contribute new features, feel free to open an issue or submit a pull request. Please follow our contribution guidelines when contributing to this project.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
