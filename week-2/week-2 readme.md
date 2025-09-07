# Garbage Classification - CNN vs Logistic Regression

This project implements **image classification** on a Garbage Dataset using two models:
- **Logistic Regression** (baseline)
- **Convolutional Neural Network (CNN)** (deep learning approach)

## 📂 Dataset
The dataset is taken from Kaggle:  
`/kaggle/input/garbage-classification-v2/garbage-dataset`

It contains multiple classes of garbage images.

## ⚙️ Models
1. **Logistic Regression**  
   - Uses flattened pixel features.  
   - Serves as a fast but simple baseline.  

2. **CNN (Convolutional Neural Network)**  
   - Lightweight architecture with Conv2D and MaxPooling layers.  
   - Achieves much better accuracy compared to logistic regression.  

## 🚀 Training
- **Fast Mode:**  
  Smaller image size (32x32), fewer epochs → faster execution.  
- **Accurate Mode:**  
  Larger images (64x64+), more epochs, stronger CNN layers → slower but higher accuracy.  

## 📊 Results
| Model                | Accuracy |
|-----------------------|----------|
| Logistic Regression   | ~X%      |
| CNN (Fast)            | ~Y%      |
| CNN (Accurate)        | ~Z%      |

## 💾 Saved Models
- `garbage_cnn_fast.h5`  
- `garbage_cnn_accurate.h5`  

## 📌 How to Run
1. Clone this repository
   ```bash
   git clone <your_repo_url>
   cd <your_repo_name>
2. Run the notebook or Python scripts in your environment (e.g., Kaggle, Colab, local Jupyter).
3. Commit the README
If local:
```bash
git add README.md
git commit -m "Added README"
git push
