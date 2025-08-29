Image Tampering Detection with CASIA 2.0

This repository contains a Jupyter Notebook for image tampering detection experiments using the CASIA 2.0 Image Tampering Dataset.

The notebook demonstrates the full workflow of:

Downloading and preparing the dataset

Preprocessing images with Error Level Analysis (ELA)

Training machine learning models to detect tampered images

Evaluating model performance with metrics and visualizations

📓 Notebook

image_tampering_CASIA2.ipynb

Implements the workflow for CASIA 2.0 dataset.
This notebook is separated from others to allow for independent experimentation and faster evaluation without re-running multiple datasets.

⚙️ Setup
1. Install dependencies
pip install torch torchvision pillow kagglehub matplotlib scikit-learn

2. Download CASIA 2.0 dataset

The notebook automatically fetches the dataset via KaggleHub
.

Alternatively, you can download from the CASIA Forensics website
.

🚀 Workflow
Preprocessing

Error Level Analysis (ELA):
Each image is resaved at 90% quality, and the difference from the original is computed. This highlights tampered regions.

Training

Models are trained using PyTorch.

Data is split into Authentic and Tampered categories.

Evaluation

Performance measured using metrics such as accuracy, precision, recall, and F1-score.

Visualizations included in the notebook for comparison of results.

📚 References

[CASIA Image Tampering Detection Evaluation Database (official site)](https://forensics.idealtest.org/)e

[CASIA 2.0 on Kaggle](https://www.kaggle.com/datasets/divg07/casia-20-image-tampering-detection-dataset)
