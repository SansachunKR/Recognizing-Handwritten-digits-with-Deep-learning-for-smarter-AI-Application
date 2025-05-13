# Handwritten Digit Recognition with Deep Learning

![MNIST Example](https://github.com/SansachunKR/handwritten-digit-recognition/raw/main/assets/mnist_example.png)

A deep learning model for recognizing handwritten digits (0-9) using convolutional neural networks.

## Features

- CNN architecture with 99%+ accuracy on MNIST
- Real-time prediction API
- Web interface for drawing digits
- Model training and evaluation scripts

## Quick Start

```bash
git clone https://github.com/SansachunKR/handwritten-digit-recognition.git 
cd handwritten-digit-recognition
pip install -r requirements.txt
python src/train.py
streamlit run app/streamlit_app.py

## Project Structure
handwritten-digit-recognition/
├── data/               # Dataset files
├── models/             # Trained models
├── notebooks/          # Jupyter notebooks
├── src/                # Source code
├── tests/              # Unit tests
├── app/                # Web application
├── assets/             # Images/samples
├── requirements.txt    # Dependencies
└── README.md           # This file

## Model Architecture :

(python)
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Conv2D, MaxPooling2D, Flatten, Dense

model = Sequential([
    Conv2D(32, (3,3), activation='relu', input_shape=(28,28,1)),
    MaxPooling2D((2,2)),
    Conv2D(64, (3,3), activation='relu'),
    MaxPooling2D((2,2)),
    Flatten(),
    Dense(128, activation='relu'),
    Dense(10, activation='softmax')
])

## Results :

Model	Accuracy	Loss	Parameters
Basic CNN	99.1%	0.03	1.2M
With Dropout	99.3%	0.02	1.3M

