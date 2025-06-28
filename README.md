# 🌾 Rice Leaf Disease Detection using Dynamic Mode Decomposition and DenseNet121

## 📌 Project Overview

Rice is a staple crop for over 3.5 billion people globally. However, its productivity is seriously affected by foliar diseases such as **Bacterial Blight**, **Leaf Blast**, **Brown Spot**, **Hispa**, and **Tungro**. Traditional disease detection methods are labor-intensive and prone to errors.

This project proposes a novel deep learning framework combining **Dynamic Mode Decomposition (DMD)** for preprocessing and **DenseNet121** for classification. DMD enhances disease-infected regions while removing background noise, improving the model's focus and classification accuracy.

---

## 🎯 Research Objectives

1. Detect and classify rice leaf diseases using deep learning.
2. Apply DMD as a preprocessing step to reduce background noise and highlight infected regions.
3. Fine-tune DenseNet121 using transfer learning for efficient feature extraction.
4. Evaluate model performance using standard metrics: **accuracy**, **precision**, **recall**, and **F1-score**.

---

## 🧪 Experimental Setup

- **Dataset Size:** 9607 labeled rice leaf images.
- **Data Split:** 80% Training, 20% Validation/Test.
- **Model:** DenseNet121 (fine-tuned with transfer learning).
- **Preprocessing:** Dynamic Mode Decomposition (DMD).
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-score.

### ✅ Achieved Performance:
| Metric         | Value     |
|----------------|-----------|
| Training Accuracy | 93.32%    |
| Validation Accuracy | 92.50% |
| Test Accuracy     | 91.59%    |

---

## 🧠 Model Architecture

### 🔹 Preprocessing – Dynamic Mode Decomposition (DMD)
- Isolates low-rank background and extracts dynamic features from the image.
- Reduces noise from soil, shadows, and lighting variations.
- Highlights affected areas before feeding into CNN.

### 🔹 Deep Learning Model – DenseNet121
- Dense connectivity improves gradient flow and feature reuse.
- Fine-tuned on the rice leaf dataset using transfer learning.
- Integrated with attention-driven DMD features for better classification.

---

## 📊 Dataset Details

- **Diseases Covered:**  
  - Bacterial Blight  
  - Leaf Blast  
  - Brown Spot  
  - Hispa  
  - Tungro

- **Format:** RGB Leaf Images  
- **Size:** 9607 images (high-quality, labeled)  
- **Source:** Custom-collected/annotated dataset  

---

## 📁 Project Structure
rice-leaf-disease-detection/
│
├── data/ # Raw dataset (train/test/val folders)
├── preprocessing/ # DMD preprocessing scripts
├── models/ # Training and inference code
├── outputs/ # Model checkpoints, confusion matrices, sample results
├── utils/ # Helper functions (visualization, metrics)
├── requirements.txt # Python dependencies
└── README.md # Project documentation (this file)


---

## ⚙️ How to Run the Project

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/rice-leaf-disease-detection.git
cd rice-leaf-disease-detection

📦 Requirements
torch>=1.10.0
torchvision
opencv-python
numpy
matplotlib
seaborn
scikit-learn
tqdm
Pillow

Install all dependencies using:
pip install -r requirements.txt
