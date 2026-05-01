# Comparative Study of CNN and Autoencoder Models for Pneumonia Detection

## Overview  
This project explores deep learning methods for detecting pneumonia from chest X-ray images. We compare two approaches:

- **Convolutional Neural Network (CNN)** – supervised learning  
- **Autoencoder (AE)** – unsupervised anomaly detection  

The goal is to evaluate performance differences between classification and reconstruction-based methods.


## Dataset  
**Chest X-Ray Images (Pneumonia)** from Kaggle  

- Classes: Normal, Pneumonia  
- Image type: Grayscale  
- Predefined train/test split  

### Preprocessing
- Resize images (e.g., 128×128 or 224×224)  
- Normalize pixel values  
- Optional validation split  



## Methods  

### CNN (Supervised)
- Convolutional layers  
- Pooling layers  
- Fully connected layers  
- Binary output (Normal vs Pneumonia)

### Autoencoder (Unsupervised)
- Encoder → latent space → decoder  
- Trained on normal images only  
- Uses reconstruction error to detect anomalies  



## Model Architectures  

**CNN:**  
Conv → ReLU → Pool → Fully Connected → Output  

**Autoencoder:**  
Input → Encoder → Latent → Decoder → Reconstruction  

---

## Results  

### CNN
- Accuracy: **86.2%**  
- Precision: **85.3%**  
- Recall: **94.1%**  
- F1-score: **89.5%**

✔ Strong performance, especially high recall (important for medical use)


### Autoencoder
- Accuracy: **58.2%**  
- Precision: **62.0%**  
- Recall: **85.4%**  
- F1-score: **71.8%**

✔ Lower accuracy but useful for anomaly detection without labels  



## Key Insights  
- CNN performs better overall  
- Autoencoder works without labeled data  
- Recall is critical to avoid missed pneumonia cases  
- Autoencoders can highlight abnormal regions  



## Visualizations  
- Confusion matrix  
- Training vs validation loss  
- Reconstruction examples  



## Future Work  
- Improve autoencoder (e.g., VAE)  
- Add data augmentation  
- Explore hybrid models  
- Test on more datasets  



## References  
- Kaggle Pneumonia Dataset  
- CNN baseline notebook  



## Team  
- Anna Andriiko
- Salena Price
- Kesler Atkinson
