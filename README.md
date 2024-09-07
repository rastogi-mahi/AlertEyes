# AlertEyes
# Drowsiness Detection Using Deep Learning

## Overview

This project implements a **drowsiness detection system** using deep learning techniques. The model is trained to distinguish between open and closed eye states from images, helping to detect signs of drowsiness in real time. 

The project leverages **Transfer Learning** with MobileNet, a lightweight neural network architecture, to achieve high accuracy on a dataset of open and closed eye images.

## Features

- **Real-Time Detection**: The system predicts if a person’s eyes are open or closed using an image input.
- **Transfer Learning**: The model uses **MobileNet** for feature extraction and adds custom layers for binary classification.
- **Evaluation Metrics**: Accuracy, precision, recall, F1-score, and a confusion matrix are used to assess model performance.

## Installation & Setup

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/drowsiness-detection.git
    ```

2. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```


## Usage

1. **Unzipping the dataset**:
   The dataset is unzipped and processed before training begins.

2. **Training the model**:
   The `main.py` script handles training the model. The images are resized, normalized, and passed into MobileNet for transfer learning. Custom layers are added for binary classification.

   Run the script to train the model:

    ```bash
    python main.py
    ```

3. **Prediction**:
   After training, the script makes predictions on a new image. It will predict whether the eye is **open** or **closed**.

## Training & Evaluation

- **Training**: The model is trained on open and closed eye images with a validation split to track performance during training.
- **Evaluation**: Various metrics such as accuracy, precision, recall, F1 score, and a confusion matrix are generated.

### Confusion Matrix Example

The confusion matrix gives insight into how well the model is predicting the classes.

### Accuracy & Loss Graphs

Training and validation accuracy/loss graphs are plotted to visualize model performance over epochs.

## Model Performance

After 5 epochs of training, the model achieves the following:

- **Accuracy**: 95%
- **Precision**: 96%
- **Recall**: 94%
- **F1-Score**: 95%

## Contributing

Feel free to submit issues or pull requests if you have ideas for improving the project.

## Acknowledgments

- The model utilizes **MobileNet** for transfer learning.
- **OpenCV** is used for image preprocessing and manipulation.


