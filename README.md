# Brain Tumor Detection using Vision Transformers (ViT)

This project implements a deep learning pipeline for brain tumor classification using Vision Transformer (ViT) models with custom patch sizes. The aim is to classify MRI scans into four categories: Glioma, Meningioma, Pituitary, and No Tumor.

## 📌 Project Overview

Brain tumor detection from MRI scans is a critical task in medical image analysis. Traditional CNN-based models have shown good performance, but Vision Transformers (ViT) offer new opportunities to capture long-range dependencies and global contextual information.

In this project, we experiment with different patch sizes (15, 12, and 20) to analyze their effect on classification accuracy and training efficiency.

## 🔬 Model Details

Architecture: Vision Transformer (ViT)  
Patch Sizes Tested:  
15 → Custom configuration  
12 → Finer-grained image features  
20 → Larger patches, faster training

## 📂 Dataset

We use the Brain MRI Images for Brain Tumor Detection dataset from Kaggle:

https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset/data

The dataset contains MRI scans classified into four categories:

* Glioma  
* Meningioma  
* Pituitary  
* No Tumor

## ⚙️ Installation & Setup

### 1. Clone the repository:

  <img width="640" height="78" alt="image" src="https://github.com/user-attachments/assets/d166d4d0-6299-4081-b0af-0660199b8f0a" />  

### 2. Install dependencies:

   <img width="553" height="69" alt="image" src="https://github.com/user-attachments/assets/467c94c8-f61d-4477-a195-b35ab8239277" />

## 🚀 Usage

### 1. Preprocess Dataset

Place dataset in data/ directory

Run preprocessing script:

<img width="523" height="62" alt="image" src="https://github.com/user-attachments/assets/618544a4-8126-4a5f-acbd-86880a068e6b" />

### 2. Train the Model 

<img width="610" height="109" alt="image" src="https://github.com/user-attachments/assets/a106d58b-f1b1-4b99-ad80-97b5b46d1580" />

### 3. Evaluate the Model

<img width="657" height="58" alt="image" src="https://github.com/user-attachments/assets/86079efe-5389-4dda-8fa9-c629aeff65bd" />

## 📊 Results
We compared the performance of ViT models trained with different patch sizes on the brain tumor dataset:

| Patch Size | Notes | Accuracy |
|------------|-------|----------|
| **12** | Finer-grained features, better detail capture | **0.8862** |
| **15** | Balanced custom configuration | **0.8558** |
| **20** | Larger patches, faster training but less detail | **0.8570** |

### Key Insights:

* Smaller patch size (12) provided the highest accuracy due to finer feature extraction.
* Larger patch size (20) sped up training but slightly reduced accuracy.
* Patch size 15 offered a balance but underperformed compared to 12.

## 📈 Future Work

* Experiment with hybrid CNN-ViT models
* Apply data augmentation for improved generalization
* Optimize hyperparameters (learning rate, batch size, optimizer)
* Explore transfer learning from pre-trained ViTs
