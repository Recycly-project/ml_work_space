# 📚 Recycly ML Workspace Documentation

## 🕵️‍♀️ Our ML Team
| Name              | Bangkit ID       |
|-------------------|------------------|
| Angelina          | M429B4KX0543       |
| Luthfi Delvian      |  M596B4KY2304      |
| Qori Alfiani Hakiki     | M179B4KX3545     |

Recycly is a machine learning-based project that classifies plastic bottles into four categories: **damaged bottles**, **recyclable bottles**, **full bottles**, and **non-bottles**. This helps improve waste sorting and encourages sustainable recycling practices.

## 📋 Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Development](#model-development)
- [Deployment](#deployment)
- [Environment Setup](#environment-setup)
- [Running Locally](#running-locally)


## 📌 Project Overview
Recycly uses a **MobileNetV2** model with transfer learning to classify plastic bottles. The goal is to improve recycling by automating waste sorting and providing rewards for proper disposal.

## 📊 Dataset
- **Classes:**  
  1. Damaged Bottles  
  2. Recyclable Bottles  
  3. Full Bottles  
  4. Non-Bottles  
- **Preprocessing:** Resized to 224x224 pixels, normalized, and augmented with random flips and rotations.

## 🚰 Model Development
- **Architecture:** MobileNetV2 (Pre-trained) with fine-tuned top layers.
- **Training:** Categorical Crossentropy loss, Adam optimizer, and early stopping for better accuracy.

## 🚀 Deployment
- **Tools Used:** TensorFlow Lite for mobile model deployment, Flask for local API server.

## 💻 Environment Setup
1. Install dependencies:
   ```bash
   pip install tensorflow flask
   ```
2. Clone the repo and run:
   ```bash
   git clone https://github.com/Recycly-project/ml_work_space.git
   cd recycly-ml-workspace
   ```

## 🏃‍♂️ Running Locally
1. Train the model:
   ```bash
   python train_model.py
   ```
2. Convert to TensorFlow Lite:
   ```bash
   python convert_to_tflite.py
   ```
3. Run the Flask app:
   ```bash
   python app.py
   ```

