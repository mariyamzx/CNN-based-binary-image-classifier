# 🐾 FurSight: CNN-Based Cats vs Dogs Classifier

A deep learning project that classifies images of cats 🐱 and dogs 🐶 using a **custom Convolutional Neural Network (CNN)** built from scratch.  
This project focuses on improving generalization through **data augmentation**, **batch normalization**, and **dropout** techniques.

---

## 📘 Overview
The model is trained on the **Dogs vs Cats** dataset from Kaggle using TensorFlow/Keras.  
It demonstrates an end-to-end workflow — from dataset loading via `kagglehub`, preprocessing, augmentation, and training, to evaluation and visual predictions.

---

## 🧩 Model Architecture
- **Input:** 256×256 RGB images  
- **3 Convolutional Blocks:** (Conv2D → BatchNorm → MaxPooling)  
- **Dense Layers:** 128 → 64 neurons  
- **Regularization:** Dropout (0.1), Batch Normalization  
- **Output:** Sigmoid activation for binary classification  

---

## 🚀 Techniques Used
- **Data Augmentation:** Random flip, brightness, contrast, and saturation adjustments  
- **Early Stopping & LR Scheduling:** To avoid overfitting and optimize convergence  
- **Batch Normalization & Dropout:** To stabilize and regularize training  
- **Prefetching & Parallelization:** For faster data loading  

---

## 📊 Results
| Metric | Score |
|:-------|:------:|
| **Training Accuracy** | ~98% |
| **Validation Accuracy** | ~95% |
| **Test Accuracy** | ~94% |

The model performs consistently well and generalizes effectively to unseen data.

---

## 📈 Visual Results

Below are sample predictions where the model correctly identifies cats and dogs with high confidence:

Pred: dog ✅
True: dog
Pred: cat ❌
True: dog



*(Use the plot generated in the notebook as a visual example — you can save it as `images/sample_predictions.png`.)*

---

## 🧠 Technologies Used
- Python 🐍  
- TensorFlow / Keras  
- Matplotlib  
- KaggleHub  
- NumPy  

---

## 💾 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/FurSight-CNN.git
   cd FurSight-CNN
Install dependencies:


pip install -r requirements.txt
Run the notebook:


jupyter notebook notebooks/FurSight_CatsDogs.ipynb
(Optional) Retrain model:


model.fit(train_ds_processed, epochs=10, validation_data=val_ds_processed)
## 🏆 Author

**Mariyam Muzammil**  
🎓 BS Computer and Information Science — PIEAS (Batch 2023–2027)  
💡 Interests: Machine Learning | Deep Learning | Computer Vision  

 
- [GitHub](https://github.com/mariyamzx)  

---

## 🪶 License

This project is open-source and available under the **MIT License**.
