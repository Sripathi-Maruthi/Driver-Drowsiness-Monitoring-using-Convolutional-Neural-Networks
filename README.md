# Driver Drowsiness Monitoring System using CNN

[![Python](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/) 
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## Project Overview
The **Driver Drowsiness Monitoring System** is an intelligent application designed to improve road safety by detecting driver fatigue in real-time. Using **Convolutional Neural Networks (CNNs)** and computer vision, the system monitors facial features, eye closure, and head movements to detect drowsiness and alert the driver immediately.

This project provides a **non-intrusive, accurate, and real-time** solution to reduce accidents caused by driver fatigue.

---

## Features
- Real-time driver monitoring using a webcam or dashcam.
- Detects signs of drowsiness:
  - Eye closure/blinking patterns
  - Yawning detection
  - Head nodding
- Instant audio alert when drowsiness is detected.
- Lightweight CNN model for fast and accurate detection.
- Easy to deploy on desktop or embedded devices.

---

## Technologies Used
- **Programming Language:** Python  
- **Deep Learning Framework:** TensorFlow / Keras or PyTorch  
- **Computer Vision Library:** OpenCV  
- **Model Architecture:** Convolutional Neural Networks (CNN)  
- **Facial Landmark Detection:** Dlib (optional)  

---

## Dataset
- Public datasets such as **CEW (Closed Eyes in the Wild)** or **YawDD**.  
- Custom labeled datasets can also be used (`drowsy` and `alert` states).  

---

## Workflow
1. Capture video frames from webcam/dashcam.
2. Detect the driver’s face and eyes using computer vision.
3. Preprocess frames (grayscale, resize, normalization).
4. Feed preprocessed frames into the CNN model to classify **drowsy vs alert**.
5. Trigger audio alert if drowsiness is detected.

---

## Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/Driver-Drowsiness-CNN.git

# Navigate to project directory
cd Driver-Drowsiness-CNN

# Install dependencies
pip install -r requirements.txt

# Run the monitoring system
python drowsiness_monitor.py
