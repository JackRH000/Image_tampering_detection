# Image Tampering Detection with CASIA 2.0

This repository contains a Jupyter Notebook for image tampering detection experiments using the CASIA 2.0 Image Tampering Dataset.

The notebook demonstrates the full workflow of:
1. Downloading and preparing the dataset
2. Preprocessing images with Error Level Analysis (ELA)
3. Training machine learning models to detect tampered images
4. Evaluating model performance with metrics and visualizations

## 📓 Notebook

- **[`image_tampering_CASIA2.ipynb`](./image_tampering_CASIA2.ipynb)**  

Implements the workflow for CASIA 2.0 dataset.
This notebook is separated from others to allow for independent experimentation and faster evaluation without re-running multiple datasets.

## ⚙️ Setup

### 1. Install dependencies

```bash
pip install torch torchvision pillow kagglehub matplotlib scikit-learn
```

### 2. Download CASIA 2.0 dataset
The notebook automatically fetches the dataset via [KaggleHub](https://www.kaggle.com/datasets/divg07/casia-20-image-tampering-detection-dataset).  

Alternatively, you can download it from the [CASIA Image Tampering Detection Evaluation Database (official site)](https://forensics.idealtest.org/).

---

## 🚀 Workflow

### Preprocessing
- **Error Level Analysis (ELA):**  
  Each image is resaved at 90% quality, and the difference from the original is computed. This highlights tampered regions.  

### Training
- Models are trained using **PyTorch**.  
- Data is split into **Authentic** and **Tampered** categories.  

### Evaluation
- Performance measured using metrics such as **accuracy, precision, recall, and F1-score**.  
- Visualizations included in the notebook for comparison of results.  

---

## 📊 Results
- Models trained on ELA-processed CASIA 2.0 images.  
- Preliminary findings:  
  - Authentic and tampered images show distinct ELA signatures.  
  - Machine learning classifiers are able to achieve strong performance.  


---

## 📚 Dataset Sources
- [CASIA Image Tampering Detection Evaluation Database (official site)](https://forensics.idealtest.org/)  
- [CASIA 2.0 on Kaggle](https://www.kaggle.com/datasets/divg07/casia-20-image-tampering-detection-dataset)  

⚠️ **Note:** The dataset itself is not included in this repository due to licensing restrictions. Please download it from one of the sources above.

---
