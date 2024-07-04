# Augmented Reality Project: Mixing Reality with Digital Information

## Project Overview

This project aims to enhance the aesthetics of a classroom by adding digital information to the physical environment using Augmented Reality (AR) technology. The goal is to overlay a digital poster onto an empty wall in classroom H238, creating a seamless blend of virtual and real-world objects.

## Project Structure

This repository contains the following folders and files:

* `code/`: Contains the Python code for the AR algorithm, including the Aruco marker detection, perspective transformation, and image merging.
* `images/`: Stores the input images used for testing the AR algorithm, including the classroom image and the poster image.
* `dataset/`: Contains the dataset used for training and testing the AR algorithm, including the Room with ArUco Markers dataset.
* `README.md`: This file, which provides an overview of the project and its components.

## Algorithm

The AR algorithm consists of the following steps:

### Aruco Marker Detection

Detect the Aruco marker in the classroom image using the OpenCV library.

### Concentric and Similar Quadrilateral Creation

Create a smaller concentric and similar quadrilateral in the poster image to match the perspective of the classroom wall.

### Perspective Matrix Calculation

Calculate the perspective transformation matrix between the quadrilaterals.

### Warp Perspective Transformation

Apply the perspective transformation matrix to the poster image to warp it into the shape of the detected Aruco marker.

### Image Merging

Merge the warped poster image with the classroom image to create a seamless AR experience.

## Dataset

The dataset used for this project is the Room with ArUco Markers dataset, which provides a set of images with Aruco markers placed in a classroom environment.

## Requirements

To run this project, you will need:

* Python 3.x
* OpenCV library
* NumPy library
* Matplotlib library (optional)

## Usage

To use this project, follow these steps:

1. Clone the repository to your local machine.
2. Install the required libraries using `pip install`.
3. Place the input images in the `images/` folder.
4. Run the `main.py` script in the `code/` folder to execute the AR algorithm.
5. View the output images in the `images/` folder.
