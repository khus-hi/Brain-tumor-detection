# Brain-tumor-detection
This project implements a deep learning pipeline for brain tumor classification using Vision Transformer (ViT) models with custom patch sizes: 15, 12, and 20. The ViT models are trained and evaluated on MRI images to detect different types of brain tumors.

We experimented with different patch sizes to evaluate their effect on classification performance:

Patch Size	 	Notes
  15		      Custom configuration
  12		      Finer-grained image features
  20		      Larger patches, faster training

**Dataset:**  We use the Brain MRI Images for Brain Tumor Detection dataset, which includes three tumor types:

1. Glioma
2. Meningioma
3. Pituitary
4. No Tumor
