# Arabic Sign-Language Recognition

This project focuses on building a deep learning model capable of recognizing Arabic Sign Language (ArSL) from video input. The model is trained to detect both **static signs** (letters and numbers) and **dynamic gestures** (18 common Arabic action verbs), aiming to bridge the communication gap for the hearing-impaired Arabic-speaking community.

## 📌 Project Overview

- **Goal:** To create a robust sign language recognition system for Arabic using computer vision and deep learning techniques.
- **Model Architecture:** Long Short-Term Memory (LSTM) networks for dynamic sequence modeling.
- **Dataset:** [KArSL dataset](https://www.kaggle.com/datasets/karim196/karasl-dataset) containing 2500+ videos across various ArSL gestures.

---

## 🧰 Technologies Used

- **Python**
- **OpenCV** – for video processing and frame extraction
- **TensorFlow / Keras** – for model building and training
- **LSTM** – to model temporal sequences of sign gestures
- **MediaPipe (optional)** – for landmark detection

---

## 📊 Results

- **Accuracy:** Achieved **98%+** accuracy across the validation set.
- **Performance:** Successfully generalized to both static and dynamic signs, making it suitable for real-time applications.

---

## 🧪 How It Works

1. **Preprocessing:**
   - Extract frames from videos
   - Use MediaPipe (or OpenCV) to detect hand landmarks
   - Normalize and reshape input for the LSTM model

2. **Model Training:**
   - Input: Sequences of landmark coordinates (or frames)
   - LSTM layers with dropout regularization
   - Output: Categorical prediction over the ArSL vocabulary

3. **Prediction:**
   - Feed real-time or test video into the model
   - Predict sign language class with softmax output

---

## 🚀 Getting Started

### Prerequisites

- Python 3.7+
- Install dependencies:
```bash
pip install -r requirements.txt
