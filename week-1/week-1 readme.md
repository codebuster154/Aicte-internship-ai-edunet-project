# 🗑️ Garbage Classification - Week 1

This is **Week 1** of the Garbage Classification project.  
The focus of this week was to **set up the dataset, preprocess images, and train a simple Logistic Regression baseline model** to verify everything is working.

---

## 📂 Dataset
The dataset used is from Kaggle:  
`/kaggle/input/garbage-classification-v2/garbage-dataset`

- Contains images from multiple garbage categories (e.g., cardboard, plastic, metal, paper, etc.).  
- Data is organized into class-wise folders.  
- Used as a supervised classification dataset.

---

## 🔎 Tasks Completed

### 1. Dataset Setup
- Loaded dataset directly from the Kaggle input path.  
- Verified the dataset structure and number of classes.  
- Displayed sample images from each class for visualization.

### 2. Preprocessing
- Rescaled pixel values to range `[0,1]` using `rescale=1./255`.  
- Resized all images to a smaller fixed size (`32x32`) for faster processing.  
- Prepared training and validation sets using `ImageDataGenerator`.

### 3. Baseline Model - Logistic Regression
- Converted images into flattened 1D vectors.  
- Trained Logistic Regression on a small subset of the data.  
- Evaluated predictions on a validation batch.  

---

## 📊 Results (Week 1)
- Logistic Regression provided only **basic baseline accuracy** (low performance).  
- Demonstrated that garbage image classification needs **deeper models like CNNs**.  
- Verified that the dataset can be successfully loaded and trained.

---

## 🚀 Next Steps
- In **Week 2**, implement a **Convolutional Neural Network (CNN)**.  
- Compare Logistic Regression vs CNN performance.  
- Create both **Fast Mode** (quick training) and **Accurate Mode** (slower but better results).

---

## 📌 How to Run
1. Open the Kaggle Notebook.  
2. Set dataset path:  
   ```python
   root_dir = "/kaggle/input/garbage-classification-v2/garbage-dataset"
3. Run the notebook step by step to reproduce Week 1 results.
