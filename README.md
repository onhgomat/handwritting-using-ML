# 🖋 Handwriting Recognition with Mini Neural Network

This is a simple **handwriting recognition project** built using a **Mini Neural Network**.  
It can recognize handwritten digits (0–9) from images, inspired by the **MNIST dataset**.

---

## 🧠 Project Overview

The goal of this project is to implement a **lightweight neural network** from scratch (without heavy frameworks) that can:

- Take an image of a handwritten digit as input.
- Process it through a mini neural network.
- Output the predicted digit (0–9).

This project is perfect for understanding:

- Forward propagation & backpropagation  
- Activation functions (Sigmoid / ReLU / Softmax)  
- Training a neural network on small datasets  
- Basic image preprocessing  

---

## ⚙️ Features

- ✅ Recognizes digits from 28x28 grayscale images  
- ✅ Mini neural network: 1 hidden layer (configurable)  
- ✅ Uses **stochastic gradient descent (SGD)** for training  
- ✅ Lightweight and easy to understand  
- ✅ Can be extended to letters or other handwritten symbols  

---

## 📝 How It Works

1. **Data Preparation**:  
   - Load MNIST dataset (or your custom handwriting images)  
   - Normalize pixel values (0–1)  

2. **Mini Neural Network**:  
   - Input layer: 784 neurons (28x28 pixels)  
   - Hidden layer: configurable (e.g., 64 neurons)  
   - Output layer: 10 neurons (digits 0–9)  
   - Activation: Sigmoid or ReLU for hidden, Softmax for output  

3. **Training**:  
   - Loss function: Cross-Entropy  
   - Optimizer: Stochastic Gradient Descent  
   - Mini-batch training  

4. **Prediction**:  
   - Forward pass on new images  
   - Output predicted digit  

---

## 💻 Installation

```bash
# Clone the repo
git clone https://github.com/your-username/handwriting-ml-mini.git
cd handwriting-ml-mini

# Install dependencies
pip install -r requirements.txt

# Run training
python train.py

# Test on your image
python predict.py --image path/to/image.png
