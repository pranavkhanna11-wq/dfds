# Deepfake Detection System

## Overview

Deepfake Detection System is a deep learning-based application designed to identify whether an image is real or AI-generated/manipulated. The project uses an EfficientNet-B4 backbone combined with advanced training techniques, data augmentation, test-time augmentation (TTA), and a Flask-based web interface for real-time predictions.

The system provides:

* Deepfake image classification
* High-accuracy deep learning model
* Interactive web dashboard
* Confidence score visualization
* Upload and analyze images through a browser
* Training, evaluation, and deployment pipeline in a single notebook

---

## Features

✅ EfficientNet-B4 based classifier

✅ Advanced image augmentation

✅ Class-balanced training

✅ Label smoothing for better generalization

✅ Mixed precision training (AMP)

✅ Test-Time Augmentation (TTA)

✅ Flask Web Application

✅ ngrok support for public deployment

✅ Prediction confidence visualization

---

## Project Structure

```text
Deepfake-Detection-System/
│
├── Deepfake_Detection_System.ipynb
├── templates/
│   ├── upload.html
│   └── dashboard.html
├── uploads/
├── saved_model/
├── README.md
└── requirements.txt
```

---

## Model Architecture

The project uses:

* EfficientNet-B4 (Primary Model)
* PyTorch Framework
* Transfer Learning
* Gradual Layer Unfreezing
* Label Smoothing BCE Loss

Input Image → EfficientNet-B4 → Classification Head → Real/Fake Prediction

---

## Dataset

The model can be trained on deepfake datasets such as:

* DFDC (DeepFake Detection Challenge)
* FaceForensics++
* Custom real/fake face datasets

Dataset images are preprocessed and augmented before training.

---

## Training Techniques

### Data Augmentation

* Horizontal Flip
* Rotation
* Color Jitter
* JPEG Compression Simulation
* Noise Injection
* Blur Transformations

### Optimization

* AdamW Optimizer
* Learning Rate Scheduling
* Weight Decay
* Mixed Precision Training

### Regularization

* Label Smoothing
* Class Balancing
* Validation Monitoring

---

## Evaluation

The model is evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* ROC Curve

Test-Time Augmentation (TTA) is used to improve prediction stability and performance.

---

## Web Application

A Flask-based web interface allows users to:

1. Upload an image.
2. Analyze whether it is real or fake.
3. View prediction confidence.
4. Access results through a simple dashboard.

The application can also be exposed publicly using ngrok.

---

## Installation

### Clone Repository

```bash
git clone https://github.com/your-username/Deepfake-Detection-System.git
cd Deepfake-Detection-System
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Run Training

Open and execute:

```bash
Deepfake_Detection_System.ipynb
```

Run all cells sequentially to:

* Load dataset
* Train model
* Evaluate performance
* Save trained weights

---

## Launch Web Application

After training:

```bash
python app.py
```

Or launch directly from the notebook using the Flask + ngrok deployment section.

---

## Example Workflow

1. Train EfficientNet-B4 model
2. Save trained weights
3. Launch Flask application
4. Upload image
5. Receive prediction:

```text
Prediction: FAKE
Confidence: 97.8%
```

---

## Technologies Used

* Python
* PyTorch
* EfficientNet-B4
* OpenCV
* NumPy
* Pandas
* Matplotlib
* Flask
* ngrok

---

## Future Improvements

* Video Deepfake Detection
* Face Tracking
* Transformer-Based Models
* Mobile Application
* REST API Deployment
* Real-Time Webcam Detection

---

## Author
Pranav Khanna
Kushal Sharma
Pranshu
Pranshu Sati
## License

This project is released under the MIT License.
