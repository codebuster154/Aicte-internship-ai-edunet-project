# 🗑️ Garbage Classification - Week 2

This is **Week 2** of the Garbage Classification project.  
The focus of this week was to **train and test models** (Logistic Regression & CNN), compare their performance, and save results.

---

## 📂 Dataset
The dataset is the same as Week 1:  
`/kaggle/input/garbage-classification-v2/garbage-dataset`

- Contains multiple garbage categories (cardboard, plastic, metal, paper, etc.).  
- Data is split into training (70%) and validation (30%) using `ImageDataGenerator`.  
- Images are resized to `32x32` for faster computation.

---

## 🔎 Tasks Completed

### 1. Preprocessing
- Used **ImageDataGenerator** for:
  - Rescaling pixel values (`1./255`)  
  - Splitting dataset into training (70%) and validation (30%)  
  - Resizing to `(32,32)`  

### 2. Logistic Regression (Improved Baseline)
- Flattened images into 1D vectors.  
- Collected ~1000 training samples for Logistic Regression.  
- Trained with `saga` solver and `max_iter=1000`.  
- Achieved measurable accuracy on validation data (better than Week 1).  

### 3. Convolutional Neural Network (CNN)
- Implemented a **light CNN** with:
  - Two convolution + pooling layers  
  - One dense hidden layer with dropout  
  - Softmax output layer  
- Compiled with **Adam optimizer** and **categorical crossentropy loss**.  
- Trained for **3 epochs** (fast training).  
- Evaluated on validation set.  

### 4. Model Comparison
- Compared Logistic Regression baseline vs CNN.  
- Plotted training & validation accuracy curves.  
- CNN clearly outperformed Logistic Regression.  

---

## 📊 Results (Week 2)

- **Logistic Regression (~1000 samples):** Low but non-zero accuracy (baseline).  
- **CNN (3 epochs):** Significantly higher accuracy, showing that CNN captures image features better.  

📈 Example plot generated:  
- Blue = CNN Training Accuracy  
- Orange = CNN Validation Accuracy  
- Red dashed line = Logistic Regression Accuracy  

---

## 🚀 Next Steps
- Add a **slower but more accurate CNN mode** (larger images, more filters, more epochs).  
- Explore **data augmentation** for improving CNN generalization.  
- Save both **fast model** and **accurate model** for later comparison.  

---

## 📌 How to Run
1. Open Kaggle Notebook.  
2. Set dataset path:  
   ```python
   root_dir = "/kaggle/input/garbage-classification-v2/garbage-dataset"
3. Run the notebook cells to:
  - Train Logistic Regression baseline
  - Train CNN model
  - Compare results

✅ The CNN model is saved as:
garbage_cnn_fast.h5


