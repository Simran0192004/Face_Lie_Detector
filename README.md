# 🔍 Lie To Me – Human Lie Detector using Kernel SVM

**Lie To Me** is a human micro-expression-based lie detection model that uses the power of **Kernel Support Vector Machine (SVM)** to classify facial cues as either *truthful* or *deceptive*. By analyzing subtle patterns in facial expressions, this project explores how machine learning can identify deception beyond human perception.

---

## 📂 Dataset

- **Source**: Micro-expression images manually labeled for prototype purposes.
- **Structure**:
  - Grayscale facial images (`.png`)
  - Labels: `truth`, `lie` in `micro_labels.csv`
  - Images resized to `64x64` and flattened for model input

---

## 🧠 Model

- **Algorithm**: Kernel SVM with RBF kernel
- **Preprocessing**:
  - Grayscale conversion (using `Pillow`)
  - Image resizing and flattening
  - Label encoding (`truth` ↔ `1`, `lie` ↔ `0`)
- **Train-Test Split**: 80/20
- **Evaluation**: Classification report + Confusion matrix

---

## 📈 Results

- Accuracy, precision, and recall scores printed
- Confusion matrix plotted using Seaborn
- Shows promising early results in detecting deception from facial expressions

---

## 🛠️ Tech Stack

- Python
- NumPy, Pandas
- Matplotlib, Seaborn
- Pillow (for image processing)
- Scikit-learn (for kernel SVM)

---

## 💡 How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/yourusername/lie-to-me
   cd lie-to-me
2. Install dependencies:
   bash
   Copy
   Edit
   pip install -r requirements.txt
3. Open the notebook:
   Copy
   Edit
   lie_detector.ipynb
   Run all cells to preprocess data, train the model, and view results.

## 🚀 Future Scope
-Integrate real micro-expression datasets with verified labels
-Use pre-trained facial emotion detectors to assist labeling
-Build a Streamlit app for real-time deception prediction

## 💬 Inspiration
"The face is the mirror of the mind, and eyes without speaking confess the secrets of the heart."
– St. Jerome

This project is a playful, experimental take on building machines that can read what people try to hide.
