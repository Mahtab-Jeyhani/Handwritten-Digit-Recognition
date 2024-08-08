# Bank Checks Recognition using ORAND-CAR Dataset

This project focuses on the recognition of handwritten digits on bank checks from the ORAND-CAR dataset. Two different methods are implemented and compared to address the challenge of recognizing sequences of handwritten digits.

## Project Overview

Handwritten digit recognition is typically performed on datasets like MNIST, which are designed for recognizing individual digits. However, this project extends the challenge to sequence recognition, aiming to develop a model that can take an image of a multi-character number and convert it into text.

## Approaches

Two distinct methods are employed in this project:

1. **Character Segmentation and Recognition**: 
   - **Objective**: Separate individual characters using image processing techniques and build a model to recognize each character independently.
   - **Details**: This approach involves detecting and extracting each digit from the image using contour detection and morphological operations. After segmentation, a pre-trained model or a custom model is used to recognize each digit separately.

2. **End-to-End Sequence Recognition using RNN**: 
   - **Objective**: Develop an end-to-end model that processes the entire line of digits without requiring character segmentation.
   - **Details**: This approach utilizes a Recurrent Neural Network (RNN) to generate the output for the entire sequence of digits. The model is trained using the Connectionist Temporal Classification (CTC) loss function, which allows the model to handle variable-length sequences and learn the alignment between the input image and the target sequence.

## Dataset

The dataset used in this project is the ORAND-CAR dataset, specifically focusing on bank checks (CAR-A and CAR-B subsets). The dataset contains images of handwritten numbers found on bank checks, which are labeled accordingly.
