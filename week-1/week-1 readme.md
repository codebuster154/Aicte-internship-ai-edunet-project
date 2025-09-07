# 🗑️ Garbage Classification – Preprocessing (30% Stage)

## 📌 Project Overview
This project focuses on **Garbage Classification using CNNs**.  
The work is divided into stages:
- **30% Stage (Week 1):** Dataset import, preprocessing, and exploratory data analysis.
- **60% Stage (Week 2):** Model building and training using CNN.
- **100% Stage (Week 3):** Final evaluation, improvements, and deployment.

This repository contains the code and analysis for the **30% completion milestone**.

---

## 📂 Dataset
- **Source:** Garbage Classification Dataset (Kaggle)  
- **Classes:** 10 categories of garbage  
- **Total Images:** ~20,000 images  
- **Train / Validation Split:** 70% Train, 30% Validation (via `ImageDataGenerator`)

---

## 🛠️ Preprocessing Steps
1. Loaded dataset from Kaggle input path.  
2. Checked dataset info using Pandas (`info()`, `describe()`, `isnull()`).  
3. Verified **class distribution** across 10 categories.  
4. Applied **ImageDataGenerator**:
   - `rescale = 1./255` (normalization)
   - `validation_split = 0.3` (split dataset into train/validation)
5. Verified dataset split:
   - **Train set:** ~15,813 images (70%)  
   - **Validation set:** ~3,949 images (30%)  

---

## 📊 Exploratory Data Analysis
- Checked **missing values** → none found ✅  
- Counted images per class.  
- Visualized **class distribution** with a bar chart.  

---

## 📑 Current Output
- Train and validation generators prepared.  
- Dataset cleaned, normalized, and ready for CNN model training.  

---

## ✅ Next Steps (60% Stage)
- Build and train a CNN model.  
- Evaluate training accuracy/loss.  
- Optimize hyperparameters for better performance.  

---

## 🚀 How to Run
1. Open the Kaggle Notebook.  
2. Add dataset path:  

   ```python
   /kaggle/input/garbage-classification-v2/garbage-dataset
  
3. Run all cells → preprocessing and dataset split will be performed

---
