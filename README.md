# ERViT: Efficient Residual Vision Transformer with Attention-Guided Dual-Level Feature Fusion for Facial Depression Recognition

This repository contains the implementation of ERViT for facial expression-based depression recognition. Traditional convolutional neural networks lack long-range dependencies among facial features, whereas vision transformers are limited in preserving fine-grained spatial details. To bridge these gaps, an Efficient Residual Vision Transformer (ERViT) is developed for facial depression recognition, designing a tailored vision transformer and EfficientNet to extract global (full-face) features, alongside a modified residual network for local (forehead, eyes, and mouth) features. Subsequently, a hierarchical attention mechanism is introduced to emphasize diagnostically relevant facial regions. Additionally, an Attention-Guided Dual-Level Feature Fusion (ADFF) strategy is employed, which selectively weights and enhances local features before combining them with global features for improved depression recognition

Preprocessing steps: OpenCV for frame extraction at five seconds interval. MTCNN for facial key points detection (face, eyes, mouth, forehead). Selective cropping of face (224x224), eyes (96x192), mouth (96x128), and forehead eyes (96x192).

<img width="1793" height="732" alt="image" src="https://github.com/user-attachments/assets/91a044fc-cd8a-41a9-801e-62fec4fe9a0b" />

# AVEC2014 Dataset
Audio-Visual Emotion Challenge 2014 (AVEC2014) dataset is a public dataset, which contains 300 videos of depressed patients. Each video has corresponding ground truth (BDI-II) scores and varied in duration from 6 to 248 seconds, recorded at 30 frames per second (fps).

# Prediction Result on AVEC2014
<img width="1753" height="290" alt="image" src="https://github.com/user-attachments/assets/c1350a7c-7f4a-475d-ab9e-7eb222bcc174" />

# Citing This Work
If you find this repository useful, please consider citing our paper:

Khan MT, Shafait F, "ERViT: Efficient Residual Vision Transformer with Attention-Guided Dual-Level Feature Fusion for Facial Depression Recognition.” Big Data Research.
