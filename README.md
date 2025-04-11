# Healthy Plant Detection Using Machine Learning

This project is a **comparative study of machine learning algorithms** for detecting healthy plants using leaf images. Our aim is to help farmers and agricultural experts make informed decisions for better crop management and reduced financial loss.

---

## Contributors

- **Pranita Chaudhary** (Assistant Professor, PCCOE, Pune)  
- **Sujata Swami** (Student, PCCOE, Pune)  
- **Adinna Thaware** (Student, PCCOE, Pune)  
- **Vipul Phatangare** (Student, PCCOE, Pune)  
- **Diksha Bhosale** (Student, PCCOE, Pune)

---

## Abstract

We explored and compared six ML algorithms:  
- **Support Vector Machine (SVM)**  
- **Decision Tree**  
- **Random Forest**  
- **AdaBoost**  
- **Gradient Boosting**  
- **XGBoost**  

Using **PCA** for dimensionality reduction, we tested them on a dataset of healthy/unhealthy plant leaves (Mango, Bell Pepper, Potato, Pongamia Pinnata). Our analysis is based on accuracy, precision, recall, and MSE.

---

## Dataset

- 5660 images from the **Plant Village Dataset**
- Categories: Healthy & Diseased leaves
- Plants: Mango, Bell Pepper, Potato, Pongamia Pinnata

---

## Methodology

### Preprocessing
- Resizing images to 128x128
- Normalization (0-1 pixel range)
- Data Augmentation (rotation, flip, zoom, shift)

### Feature Extraction
- Raw images converted to numerical data
- **PCA** reduced features from 49152 → 50

### Models Used
- Traditional: **SVM, Decision Tree**
- Ensemble: **Random Forest, AdaBoost, Gradient Boosting, XGBoost**
- Custom: **Custom Boosting using multiple SVMs**

---

## Results

| Model              | Test Accuracy | F1-Score | MSE     |
|-------------------|---------------|----------|---------|
| SVM               | **93.63%**    | **0.930**| **0.0636** |
| Random Forest     | 82.27%        | 0.785    | 0.1773  |
| Decision Tree     | 80.74%        | 0.895    | 0.1926  |
| AdaBoost          | 89.22%        | 0.885    | 0.1337  |
| XGBoost           | 86.63%        | 0.855    | 0.1078  |
| Gradient Boosting | 86.69%        | 0.855    | 0.1331  |
| Custom SVM Boost  | 89.16%        | 0.885    | 0.1084  |

---

## Conclusion

The **SVM algorithm** proved to be the most effective with the highest accuracy and lowest MSE. Ensemble techniques like AdaBoost and the **custom SVM boosting model** also performed competitively. This system can be beneficial for **early disease diagnosis** and improving **agricultural productivity**.

---

## References

Citations include works from IEEE and peer-reviewed publications on plant disease detection using ML and image processing.

---

## Demo / Visualization

🖼️ Dataset samples, model architecture diagrams, and result visualizations can be found in the notebook:  
`Plant_leaf_healthy_detection.ipynb`

---

## Future Work

- Integrating Deep Learning models (CNN, ResNet, etc.)
- Expanding dataset for more crops
- Creating a web/mobile-based real-time detection system

---
