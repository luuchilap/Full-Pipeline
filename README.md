# Note:
In case cannot see the code, you can access this Google Colab link: https://drive.google.com/drive/folders/1ZiD_Iu3k_ilTy99rhF1PBD_XGqO10Vy5?usp=drive_link

This project involves building a Scene Text Recognition system using pretrained models YOLOv8 and CRNN. It covers the entire pipeline from data preparation, model training, to evaluation, ensuring the system can detect and recognize text in natural scene images effectively.
The project uses **YOLOv8** for text detection and **CRNN** for text recognition.

# **Part I: Introduction**

•	Objective: Recognize text in natural scene images.

•	Applications: Text processing in documents, information retrieval from online images, and automation tasks like order processing and payment.

•	Stages:

o	Text Detection (Detector – YOLOv8): Locating text within an image.

o	Text Recognition (Recognizer - CRNN): Identifying the text found.

# **Part II: Program Implementation**

**Phase 1: Data Preparation**

1.	Dataset Download: The project uses the ICDAR2003 dataset.

2.	Text Detection Module:

•	Library Installation: Install necessary libraries like ultralytics for YOLOv8.

•	Data Preparation:

o	Extract relevant information from XML files in ICDAR2003.

o	Convert data to the YOLOv8 format, with normalized bounding box coordinates.

o	Save the prepared data into appropriate folders for training, validation, and testing.

o	Create a data.yaml file to manage paths and class names.

**Phase 2: Model Training**

•	Text Detection: Train YOLOv8 model using the prepared dataset.

•	Evaluation: Evaluate the trained model to validate performance.

**Phase 3: Text Recognition**

1.	Data Preparation: Extract images containing only text and corresponding string labels from ICDAR2003.

2.	Model Selection: Use Convolutional Recurrent Neural Networks (CRNN) to handle the image and sequential nature of the data.
  
3.	Implementation:
   
    •	Import necessary libraries.
  	
    •	Prepare the dataset for training the CRNN model.

# Link Google Colab: 

+Text Detection: https://colab.research.google.com/drive/1DIk5Z7ZVe2_e9RskvV7Pl9YcRTMAod6H

+Text Recognition: https://colab.research.google.com/drive/1yL-iA_Z7qwoWRnwbJEQiJjMvf0swtNIU

+Full Pipeline: https://colab.research.google.com/drive/1eUbLi7Yuqk0OXOMPcr9aAS2yaQN3T-zY
