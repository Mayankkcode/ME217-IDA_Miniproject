# ME217-IDA_Miniproject
# 🛠️ Bearing Fault Detection using Vibration Signal Analysis

This project focuses on detecting faults in ball bearings through signal processing and machine learning. Vibration data is used to extract key features in the time and frequency domains, which are then used to classify different fault conditions.

---

## 📌 Objective

- Analyze vibration signals to classify the condition of ball bearings.
- Use signal processing techniques and machine learning to automate fault detection.
- Predict the condition of unknown test samples and evaluate performance using the **F1 Score**.

---

## ⚙️ Fault Conditions Considered

- **Healthy_3_0** – No fault under 3 kW load
- **BallFault_0007** – Ball fault with 0.007" diameter
- **BallFault_00028** – Ball fault with 0.028" diameter
- **Innerfault_0007** – Inner race fault with 0.007" diameter
- **Innerfault_00028** – Inner race fault with 0.028" diameter

---

---

## 🔍 Methodology

### 1. **Data Preprocessing**
- Loaded vibration data from Excel files.
- Normalized and segmented the time-series signals.

### 2. **Feature Extraction**
- **Time-Domain Features**:
  - Mean, RMS, Standard Deviation
  - Skewness, Kurtosis
  - Crest Factor, Peak-to-Peak

- **Frequency-Domain Features**:
  - FFT of signal segments
  - Dominant frequencies and corresponding magnitudes

### 3. **Model Training**
- Used classifiers like:
  - Random Forest
  - Support Vector Machine (SVM)
  - Logistic Regression (or others as applicable)
- Performed training on `extracted_features_train`

### 4. **Testing & Evaluation**
- Loaded test features from `extracted_features_test`
- Predicted conditions using trained model
- Evaluated predictions against `Actual_1.xlsx` using **F1 Score**

---

## 📊 Results

| Metric        | Value     |
|---------------|-----------|
| F1 Score      |    95.29%
| Accuracy      | 95.71%  
> Replace with actual results after model evaluation

🧠 Skills Demonstrated
Signal Processing (FFT, Time-Domain analysis)

Machine Learning (Classification, Model Evaluation)

Data Preprocessing and Feature Engineering

Performance Metrics: F1 Score, Accuracy


