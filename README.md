# 🎬 Sentiment Analysis Web App  
### Using PyTorch and Amazon SageMaker

This project is a part of the **Deep Learning Nanodegree Program | Deployment** and demonstrates how to build, train, deploy, and serve a machine learning model using **Amazon SageMaker**. The model performs **sentiment analysis** on movie reviews, predicting whether the sentiment is positive or negative.

The final product includes a simple web interface where users can input a movie review and receive real-time sentiment predictions from a SageMaker-hosted model.

---

## 🚀 Project Overview

### Objective:
To build an **end-to-end sentiment analysis system** that:
- Trains a sentiment classifier using PyTorch
- Deploys the model with Amazon SageMaker
- Serves predictions through a custom Flask-based web application

### Input:
- Text reviews submitted by users via a web interface

### Output:
- Sentiment prediction: **Positive** or **Negative**

---

## 🧭 Project Workflow

The project follows a modified version of the standard SageMaker ML pipeline:

1. **Data Acquisition**  
   - Download IMDb movie review dataset.

2. **Data Preprocessing**  
   - Clean, tokenize, and convert text to numerical format.
   - Store and manage preprocessed data locally before uploading to S3.

3. **Data Upload to S3**  
   - Upload the processed dataset to an S3 bucket to be used for training.

4. **Model Training (PyTorch + SageMaker)**  
   - Use a custom PyTorch model script for binary sentiment classification.
   - Train using SageMaker’s managed training infrastructure.

5. **Model Deployment**  
   - First deploy using SageMaker’s default predictor.
   - Then re-deploy using a custom inference script (`inference.py`) for real-time prediction.

6. **Model Testing**  
   - Use the deployed endpoint to test predictions with sample reviews.

---

## 🛠️ Tools & Technologies

- **Amazon SageMaker**
- **PyTorch**
- **Flask**
- **Boto3 (AWS SDK for Python)**
- **HTML/CSS (for the front-end)**
- **Jupyter Notebook (for development and experimentation)**

---

## 🧪 Model Details

- **Architecture**: LSTM-based binary text classifier
- **Loss Function**: Binary Cross Entropy
- **Optimizer**: Adam
- **Training Data**: IMDb Movie Review Dataset (pre-tokenized)

---

### 📈 Future Improvements
Add support for more languages

Improve front-end interface and UX

Add confidence score in predictions

Extend model to multi-class sentiment classification

👤 Author
Waqar Ahmed
📧 waqar.nu@gmail.com
🔗 GitHub (https://github.com/waqar-ahmed91)

📜 License
This project is for educational purposes only. Model and data usage are governed by their respective licenses.
