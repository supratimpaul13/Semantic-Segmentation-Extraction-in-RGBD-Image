# Semantic Segmentation and Scene Understanding using RGBD Data

This repository contains the code and documentation for the project "Semantic Segmentation and Scene Understanding using RGBD Data." The project focuses on improving the accuracy of semantic segmentation in indoor environments using RGBD data captured by the Microsoft Kinect sensor.

## Overview

Semantic segmentation is a crucial task in computer vision, aimed at classifying each pixel in an image into predefined categories. Traditional RGB-based semantic segmentation struggles with accuracy in complex, cluttered environments where objects overlap or vary in distance. Our project addresses these challenges by integrating depth information with RGB data to enhance scene understanding.

## Key Features

- **Model**: Utilizes the YOLOv8 model for efficient and accurate object detection and segmentation.
- **Data**: Combines RGB and depth images to improve segmentation performance in cluttered indoor environments.
- **Techniques**: Includes data augmentation, custom preprocessing, and depth-based spatial analysis.
- **Analysis**: Analyzes spatial and depth relationships to determine object positions and interactions.

## Results

The model achieved high precision (93.5%) and recall (97.6%) in segmenting and identifying objects such as cans, boxes, and cups. Detailed results and evaluations are available in the project paper linked below.

## Paper

For more detailed information, please refer to our project paper: [Paper](https://drive.google.com/file/d/14zRm2D6c6_pXXc6uxdt4vtg2K0wx7MaQ/view?usp=sharing)

## Dataset

The dataset consists of RGB and depth images captured in various indoor settings. It includes:
- Raw images: 153 RGB images and 153 depth images.
- Multi-object images: 25 RGB images and 25 depth images.

Each image was augmented by horizontal flipping, resulting in a total of 640 images, each resized to 415x415 pixels.

## Methodology

1. **Depth Camera Input**: Captures RGBD images using a depth camera.
2. **Scene Representation**: Separates RGB and depth information from the captured data.
3. **Semantic Segmentation**: Applies the YOLOv8 model to identify and label objects within the images.
4. **Positional Relation Calculation**: Analyzes depth and spatial relationships to determine object positions.

## Installation

To run this project, you will need to install the following dependencies:

```bash
%pip install ultralytics==8.0.196

pip install tensorflow opencv-python numpy matplotlib

from IPython import display
display.clear_output()

import ultralytics
ultralytics.checks()

from ultralytics import YOLO
from IPython.display import display, Image
```

## Usage

To run this project, you will need to install the following dependencies and run the cells of notebook:

```bash
git clone https://github.com/supratimpaul13/Semantic-Segmentation-and-Scene-Understanding-using-RGBD-Data.git
```
