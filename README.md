# Human Body Measurement Tool

This project provides a set of Python functions to perform various human body measurements from images using the `tf_bodypix` and `OpenCV` libraries. It leverages pose estimation and segmentation to derive body dimensions such as hip width, upper leg width, waist height, and crotch-to-waist height.

## Features

* **Hip Width Calculation**: Measures the hip width from a front-facing image.
* **Front Upper Leg Width**: Estimates the width of the upper leg from a front-facing image.
* **Side Upper Leg Width**: Calculates the width of the upper leg from a side profile image, automatically detecting the facing direction (left or right).
* **Scale Generation**: Determines a pixel-to-real-world scale factor using a known real height and corresponding pixel height from an image.
* **Waist Height Estimation**: Estimates the waist height based on shoulder and ankle keypoints and the user's gender.
* **Crotch-to-Waist Height Calculation**: Measures the distance from the crotch to the estimated waist height.

## Installation

To set up the environment and install the necessary libraries, run the following pip command:

```bash
pip install tf_bodypix tfjs_graph_converter opencv-python matplotlib
```

## Usage

The main functionalities are encapsulated in Python functions. You will need images of a person (front and side profiles) to use these functions.