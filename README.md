# ✍️ Handwritten Digit Recognition using CNN

A deep learning project that recognizes handwritten digits (0–9) using a Convolutional Neural Network (CNN) trained on the MNIST dataset. The model is deployed through a Gradio web interface, allowing users to draw digits and receive real-time predictions.

---

## 📖 Overview

This project demonstrates the complete machine learning workflow:

- Data preprocessing
- CNN model development
- Model training and evaluation
- Saving and loading trained models
- Interactive deployment using Gradio

Users can draw a handwritten digit on a sketchpad, and the model predicts the digit along with confidence scores.

---

## 🚀 Features

- Handwritten digit recognition
- CNN-based image classification
- MNIST dataset training
- Real-time predictions
- Interactive Gradio UI
- Confidence score display
- Easy-to-use web application

---

## 🛠️ Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pillow (PIL)
- Gradio

---

## 📂 Dataset

The project uses the MNIST dataset, a standard benchmark dataset for handwritten digit recognition.

Dataset Statistics:

- 60,000 Training Images
- 10,000 Testing Images
- 10 Classes (Digits 0–9)
- Image Size: 28 × 28 pixels

---

## 🧠 Model Architecture

Input Layer (28×28×1)

↓

Conv2D (32 Filters, 3×3, ReLU)

↓

MaxPooling2D (2×2)

↓

Flatten

↓

Dense (128 Neurons, ReLU)

↓

Dense (10 Neurons, Softmax)

↓

Digit Prediction (0–9)

---

## ⚙️ Training Configuration

| Parameter | Value |
|------------|--------|
| Optimizer | Adam |
| Loss Function | Categorical Crossentropy |
| Epochs | 5 |
| Batch Size | 128 |
| Validation Split | 10% |

---

## 📊 Workflow

### 1. Load Dataset

The MNIST dataset is loaded directly from TensorFlow.

### 2. Data Preprocessing

- Normalize pixel values
- Reshape images for CNN input
- Convert labels using one-hot encoding

### 3. Model Training

The CNN model is trained on handwritten digit images to learn visual patterns.

### 4. Save Model

The trained model is saved as:

```python
mnist_model.h5
```

### 5. Prediction Interface

A Gradio web application loads the saved model and predicts digits drawn by the user.

---

## 🌐 Running the Project

### Install Dependencies

```bash
pip install tensorflow gradio pillow numpy
```

### Train the Model

```bash
python train_model.py
```

### Launch the Application

```bash
python digit_predictor.py
```

The Gradio interface will open in your browser.

---

## 📸 Application Preview

Add screenshots here:

- Drawing Canvas
- Prediction Results
- Confidence Scores

Example:

```text
screenshots/
├── interface.png
├── prediction.png
```

---

## 🎯 Learning Outcomes

Through this project, I gained experience in:

- Deep Learning Fundamentals
- Convolutional Neural Networks (CNNs)
- Image Classification
- TensorFlow/Keras Model Development
- Data Preprocessing
- Model Deployment using Gradio
- Interactive AI Applications

---

## 📈 Future Enhancements

- Improve model accuracy with deeper CNN architectures
- Support custom handwritten datasets
- Deploy on cloud platforms
- Add real-time drawing recognition
- Display prediction confidence charts

---

## 👩‍💻 Author

**Asmitha S**

B.Tech – Artificial Intelligence & Data Science

LinkedIn: https://www.linkedin.com/in/asmitha-seenivasagam/

---
⭐ If you found this project useful, consider giving it a star!
