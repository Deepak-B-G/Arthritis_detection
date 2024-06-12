# Arthritis Detection Using CNN and Flask

This project aims to detect the severity of knee osteoarthritis using deep learning techniques. It uses a Convolutional Neural Network (CNN) for image classification and Flask to create a web application for uploading and diagnosing knee X-ray images.

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Model Details](#model-details)
- [Web Application](#web-application)
- [Results](#results)


## Introduction

Arthritis is a common condition that causes pain and inflammation in a joint. Knee osteoarthritis is the most common form of arthritis, especially among older adults. This project leverages Convolutional Neural Networks (CNNs) to classify knee X-ray images into different categories of severity, ranging from normal to severe. The web application built with Flask allows users to upload X-ray images and get a diagnosis.

## Project Structure

- `Digital Knee X-ray Images/`: Contains the dataset of knee X-ray images.
- `static/`: Contains static files like CSS and JavaScript.
- `templates/`: Contains the HTML templates for the web application.
- `Test_samples/`: Directory for test sample images.
- `uploads/`: Directory where uploaded images are stored.
- `app.py`: Main Flask application.
- `model.h5`: Pre-trained CNN model for classification.
- `Model_Training.ipynb`: Jupyter notebook for training the model.
- `README.md`: This README file.
- `requirements.txt`: List of Python dependencies.

## Prerequisites

- Python 3.x
- pip (Python package installer)

## Installation

1. Clone the repository:

```sh
git clone https://github.com/yourusername/Arthritis_detection.git
cd Arthritis_detection

```

2. Install the required packages:

```sh
pip install -r requirements.txt
```

3. Place the pre-trained model (model.h5) in the root directory of the project.

## Usage
Run the Flask application:
```sh
python app.py
```
Open your web browser and navigate to http://127.0.0.1:5000/.

Upload a knee X-ray image and click "Predict!" to get the diagnosis.

## Model Details

The CNN model is trained on a dataset of knee X-ray images. It classifies images into five categories:

1. Normal
2. Doubtful
3. Mild
4. Moderate
5. Severe

The model architecture and training details can be found in the training notebook (Model_Training.ipynb).

## Web Application
The web application is built using Flask. It allows users to upload knee X-ray images and receive a diagnosis based on the trained CNN model.

1. HTML (index.html)
The HTML template provides the user interface for uploading images and displaying results.

2. CSS (main.css)
The CSS file styles the web application, providing a clean and modern look.

3. JavaScript (main.js)
The JavaScript file contains client-side logic to enhance user interaction.

4. Flask (app.py)
The Flask application handles the backend logic, including loading the model, processing images, and making predictions.

## Results
The application classifies knee X-ray images into different severity levels of osteoarthritis with high accuracy. The results are displayed on the web interface after the image is processed by the model.



