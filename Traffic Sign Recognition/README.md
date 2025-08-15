# 🚦 Traffic Sign Recognition — Deep Learning Project

## 📌 Project Overview
This project focuses on building a **deep learning-based traffic sign classification system** capable of accurately identifying various road signs from image data.  
It is designed for **transportation and autonomous systems** where real-time, reliable recognition of road signs is critical for safety.

The model is trained on the **German Traffic Sign Recognition Benchmark (GTSRB)** dataset, a widely used benchmark in the field of computer vision for traffic sign classification.

---

## 🎯 Objectives
- Develop a **high-accuracy multi-class classification model** for traffic sign images.
- Implement **data preprocessing** and **augmentation** techniques to enhance model robustness.
- Evaluate and compare different CNN architectures.
- Provide visual analysis through **confusion matrices** and performance metrics.

---

## 📂 Dataset
- **Source:** [GTSRB Dataset on Kaggle](https://www.kaggle.com/datasets/valentynsichkar/traffic-signs-preprocessed)
- **Number of Classes:** 43 traffic sign categories.
- **Data Format:** RGB images with varying dimensions (resized during preprocessing).

---

## 🛠 Tools & Libraries
- **Languages:** Python  
- **Libraries:**
  - `TensorFlow` / `Keras` — Model development
  - `OpenCV` — Image preprocessing
  - `NumPy`, `Pandas` — Data manipulation
  - `Matplotlib`, `Seaborn` — Visualization
  - `Scikit-learn` — Evaluation metrics

---

## 📊 Methodology

### 1️⃣ Data Preprocessing
- **Image resizing** to a fixed dimension for consistency.
- **Pixel normalization** to improve training stability.
- **Data augmentation**:
  - Random rotations
  - Zoom
  - Shifts
  - Brightness adjustments

### 2️⃣ Model Development
- Designed a **custom Convolutional Neural Network (CNN)** architecture.
- Tuned hyperparameters such as learning rate, batch size, and optimizer.
- Applied **Dropout layers** to prevent overfitting.

### 3️⃣ Model Evaluation
- Accuracy score on validation and test sets.
- Confusion matrix visualization for class-level performance.
- Cross-validation to ensure model generalization.

---

## 📈 Results
| Metric              | Score   |
|---------------------|---------|
| Training Accuracy   | ~99%    |
| Validation Accuracy | ~97%    |
| Test Accuracy       | ~96%    |

*Results may vary based on hyperparameters and random seed.*

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/2bahaa/traffic-sign-recognition.git
cd traffic-sign-recognition

## 2️⃣ Install dependencies
```bash
pip install -r requirements.txt

## 3️⃣ Train the model
```bash
python train.py

## 4️⃣ Evaluate the model
```bash
python evaluate.py

## 5️⃣ Run inference on a single image
```bash
python predict.py --image_path path_to_image.jpg

## 📌 Industry Applications

Autonomous Vehicles — Real-time road sign detection for navigation.

Driver Assistance Systems — Alerts and decision support for human drivers.

Traffic Management Systems — Automatic logging and classification of road sign data.

## 📎 References

GTSRB Benchmark Dataset

Kaggle GTSRB Dataset

🙏 Acknowledgment

This project was developed during my Machine Learning Engineer Internship at Elevvo Pathways as part of an industry-level application in computer vision and intelligent transportation systems.
