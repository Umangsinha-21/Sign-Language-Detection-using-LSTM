# 🤟 Sign Language Detection using LSTM & MediaPipe

A deep learning project that recognizes sign language gestures from video input using LSTM neural networks and MediaPipe hand tracking.

---
<img width="637" height="502" alt="Image" src="https://github.com/user-attachments/assets/04c0ad74-9f06-41e8-91e5-2e02c97f908e" />
<img width="637" height="500" alt="Image" src="https://github.com/user-attachments/assets/62acaee2-b7e1-44ac-a72d-1cc07c48fddc" />
---

## 🧠 Overview

This project is focused on **Sign Language Recognition** using **Long Short-Term Memory (LSTM)** networks. It leverages **video input** to detect and classify sign language gestures into corresponding characters or words. The system uses **MediaPipe** for real-time hand landmark extraction and builds a gesture sequence model using **Keras** with TensorFlow backend.

---

## 🚀 Features

* Real-time sign language recognition
* LSTM-based sequence modeling
* Hand landmark detection using MediaPipe
* Video frame preprocessing using OpenCV
* Trained model serialization and inference
* Custom module for data preprocessing and training functions

---

## 🧰 Tech Stack & Libraries Used

| Tool/Library               | Purpose                                       |
| -------------------------- | --------------------------------------------- |
| Python                     | Core programming language                     |
| OpenCV                     | Video frame capture & preprocessing           |
| MediaPipe                  | Hand tracking & landmark detection            |
| Keras (TensorFlow backend) | LSTM model building, training, and evaluation |
| NumPy                      | Numerical operations                          |
| scikit-learn               | Dataset splitting and preprocessing           |
| TensorBoard                | Model training visualization                  |

---

## 📁 Folder Structure

```
SignLanguageDetection/
│
├── Image/                     # Collected video sequences for each gesture
├── MP_Data/                   # Saved model architecture and weights
├── function.py                # Utility functions for preprocessing and model training
├── app.py                     # Main file for training and inference
├── collecteddata.py             
├── data.py
├── model.h5
├── model.json
├── tempCodeRunnerFile.py
├── trainmodel.py
├── Research paper
├── synopsis             
├── README.md                  # Project documentation
```

---

## 📊 Power BI Dashboard

The Power BI dashboard provides a visual summary of:

* Training vs validation accuracy/loss
* Class-wise prediction performance
* Frame-wise gesture prediction timeline
* Confusion matrix for model accuracy

Data for the dashboard was exported post-training and visualized for performance insights.

---

## 🧪 How It Works

1. **Hand Landmark Extraction**:
   MediaPipe captures 21 3D hand landmarks per frame.

2. **Sequence Formation**:
   30 frames per gesture are stored as a single sequence.

3. **Model Architecture**:
   The model uses stacked LSTM layers followed by Dense layers for classification.

4. **Training & Evaluation**:
   Model trained using categorical cross-entropy loss and monitored using TensorBoard.

5. **Inference**:
   Real-time classification of gestures using live webcam feed.

---

## 🛠️ Functions Used

Some key functions from `function.py`:

* `extract_keypoints()`: Extracts 21x3 MediaPipe keypoints from each frame.
* `load_sequences()`: Loads training sequences and labels.
* `create_model()`: Defines and compiles the LSTM model.
* `train_model()`: Trains and saves the model using provided sequences.

---

## 📌 Future Work

* Expand gesture dataset for full ASL coverage
* Add word-level prediction using phrase modeling
* Deploy as a web app using Streamlit or Flask

---
## 📬 Contact

For feedback, suggestions, or collaboration:
**Umang Sinha**
* 💼 [LinkedIn](https://www.linkedin.com/in/umang-sinha-2b1853241)
* 📧 [G-Mail](umang.2003@gmail.com)

---

