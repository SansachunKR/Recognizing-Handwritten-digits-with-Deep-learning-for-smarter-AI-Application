# Handwritten Digit Recognition with Deep Learning

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![TensorFlow 2.x](https://img.shields.io/badge/TensorFlow-2.x-FF6F00.svg)](https://www.tensorflow.org/)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-CNN-9cf.svg)

A CNN-based model that achieves **99%+ accuracy** on MNIST digit classification, enabling smarter AI applications.

<p align="center">
  <img src="https://github.com/username/handwritten-digit-recognition/raw/main/assets/demo.gif" width="300" alt="Live Demo">
</p>

## Features
- 🎯 **99.2% Test Accuracy** with optimized CNN architecture
- 📊 Real-time prediction via CLI/web interface
- 🔍 Integrated Grad-CAM visualization for model interpretability
- 🚀 Ready for deployment with Docker/Flask

## Quick Start

### Prerequisites
```bash
git clone https://github.com/username/handwritten-digit-recognition.git
cd handwritten-digit-recognition
pip install -r requirements.txt
Train the Model
bash
python train.py --epochs 15 --batch_size 64
Predict on Custom Images
bash
python predict.py --image samples/test_5.png
Project Structure
handwritten-digit-recognition/
├── models/               # Saved model weights
├── notebooks/            # Jupyter notebooks for exploration
├── samples/              # Test images
├── src/
│   ├── train.py          # Training script
│   ├── predict.py        # Inference script
│   └── model.py          # CNN architecture
├── app.py                # Flask web interface
├── requirements.txt
└── README.md
Model Architecture
python
model = Sequential([
    Conv2D(32, (3,3), activation='relu', input_shape=(28,28,1)),
    MaxPooling2D((2,2)),
    Conv2D(64, (3,3), activation='relu'),
    MaxPooling2D((2,2)),
    Flatten(),
    Dense(128, activation='relu'),
    Dropout(0.5),
    Dense(10, activation='softmax')
])
Performance Metrics
Metric	Score
Accuracy	99.23%
Precision	99.31%
Recall	99.18%
F1-Score	99.24%
Live Demo
Open in Streamlit

License
This project is licensed under the MIT License.


### Key Visual Elements Included:
1. **Shields.io badges** for quick project metadata
2. **Animated demo GIF** (replace with your actual demo)
3. **Table format** for performance metrics
4. **Code blocks** with syntax highlighting
5. **Directory tree visualization**
6. **Clickable badges** for live demo

For best results:
1. Add actual screenshots/GIFs in an `/assets` folder
2. Replace placeholder URLs with your actual project links
3. Update model metrics with your real evaluation scores
