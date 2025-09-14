# 🗑️ Garbage Classification App

This is a simple web application built with **Streamlit** and **TensorFlow/Keras** that classifies uploaded images of garbage into different categories. It helps identify the type of waste and provides warnings for possible misclassifications.  

---

## **Features**

- Upload images in `.jpg`, `.jpeg`, or `.png` format.
- Classifies images into one of the following categories:
  - Cardboard
  - Glass
  - Metal
  - Paper
  - Plastic
  - Trash
---

## **Installation**

1. **Clone the repository**:
    ```bash
    git clone <your-repo-url>
    cd <repo-folder>
    ```

2. **Create a virtual environment** (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # Linux/Mac
    venv\Scripts\activate     # Windows
    ```

3. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Download the trained model**  
   Make sure your trained model file (`garbage_cnn_week3.h5`) is in the same folder as `app.py`.

---

## **Running the App**

Run the Streamlit app with the following command:

```bash
streamlit run app.py
