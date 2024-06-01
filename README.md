This project involves building a Scene Text Recognition system using pretrained models YOLOv8 and CRNN. It covers the entire pipeline from data preparation, model training, to evaluation, ensuring the system can detect and recognize text in natural scene images effectively.
The project uses YOLOv8 for text detection and CRNN for text recognition.
Part I: Introduction

Objective: Recognize text in natural scene images.

Applications: Text processing in documents, information retrieval from online images, and automation tasks like order processing and payment.

Stages:

Text Detection (Detector): Locating text within an image.

Text Recognition (Recognizer): Identifying the text found.

The project uses YOLOv8 for text detection and CRNN for text recognition.


Part II: Program Implementation

Phase 1: Data Preparation

Dataset Download: The project uses the ICDAR2003 dataset.

Text Detection Module:

Library Installation: Install necessary libraries like ultralytics for YOLOv8.

Data Preparation:

Extract relevant information from XML files in ICDAR2003.

Convert data to the YOLOv8 format, with normalized bounding box coordinates.

Save the prepared data into appropriate folders for training, validation, and testing.

Create a data.yaml file to manage paths and class names.

Phase 2: Model Training

Text Detection: Train YOLOv8 model using the prepared dataset.

Evaluation: Evaluate the trained model to validate performance.

Phase 3: Text Recognition

Data Preparation: Extract images containing only text and corresponding string labels from ICDAR2003.

Model Selection: Use Convolutional Recurrent Neural Networks (CRNN) to handle the image and sequential nature of the data.
Implementation:
Import necessary libraries.
Prepare the dataset for training the CRNN model.
