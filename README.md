# Statistical-Data-Analysis
Data Analysis in python
# **Predicting the Virulence of Bacterial Pathogens**

## 🌟 Overview
Emerging infectious diseases caused by bacterial pathogens pose a critical threat to global health. This project employs advanced machine learning techniques to predict bacterial pathogen virulence using ecological, genomic, and clinical data. By analyzing key factors like tissue tropism and transmissibility, this study provides actionable insights for clinicians, researchers, and public health experts.

Key objectives:
- Predict virulence levels of bacterial pathogens.
- Identify significant ecological and transmission-related features.
- Develop robust machine learning models for classification and analysis.

---

## 📊 Dataset Description
| **Attribute**            | **Details**                                                                                 |
|---------------------------|---------------------------------------------------------------------------------------------|
| **Source**                | Publicly available genomic, clinical, and epidemiological datasets.                        |
| **Pathogens Analyzed**    | 76 bacterial pathogens from 36 families.                                                   |
| **Severity Measures**     | Two distinct severity classifications: "Severe" and "Non-Severe".                          |
| **Preprocessing Steps**   | - Upsampling for balanced data.<br>- Feature encoding.<br>- Splitting into training (67%) and test (33%). |

---

## 🛠️ Technologies Used
| **Component**                | **Details**                                    |
|-------------------------------|-----------------------------------------------|
| **Programming Language**      | Python                                       |
| **Libraries**                 | - scikit-learn<br>- pandas<br>- NumPy<br>- Lime (for interpretability)<br>- Matplotlib and seaborn for visualizations |
| **Tools and Frameworks**      | - Jupyter Notebook<br>- GitHub for collaboration |

---

## 🚀 Features
### **1. Machine Learning Models**
| Model                          | Description                                                                                               | Strengths                                                                                           |
|--------------------------------|-----------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| **Random Forest Classifier**   | Combines decision trees for robust classification.                                                        | High precision and interpretability.                                                               |
| **Gradient Boost Classifier**  | Sequentially optimizes weak learners to improve accuracy.                                                 | Effective for imbalanced data.                                                                     |
| **Support Vector Machines**    | Separates classes with a maximum margin hyperplane.                                                      | Suitable for smaller datasets.                                                                     |
| **Linear Regression**          | Uses linear relationships for prediction.                                                                | Best for basic trends but limited in handling complex patterns.                                    |

---

### **2. Data Analysis**
- **Feature Importance**: 
  - Extracts key contributors to pathogen virulence.
  - Visualized with bar charts for easy interpretation.
- **Evaluation Metrics**:
  - Precision, Recall, F1 Score, AUC-ROC curve, and Confusion Matrices.

### **3. Interactive Visualizations**
- **LIME Interpretability Plots**:
  - Understand individual predictions and their contributing features.
- **Feature Importance Heatmap**:
  - Displays the impact of each feature on model predictions.
- **Confusion Matrix**:
  - Visualizes the performance of models in terms of predicted vs. actual classes.


---

## 🔍 Analytical Questions Explored
1. **What ecological and transmission factors strongly influence bacterial pathogen virulence?**
2. **How does tissue tropism correlate with severity levels?**
3. **What model provides the best prediction accuracy, and why?**
4. **How do upsampling and feature encoding improve model performance?**
5. **Which pathogens are misclassified, and what are the reasons?**

---

## 📈 Results and Insights
| **Model**                       | **Precision** | **Recall** | **F1 Score** | **AUC-ROC** | **Best Use Case**                                                                                  |
|---------------------------------|---------------|------------|--------------|-------------|-----------------------------------------------------------------------------------------------|
| Random Forest Classifier        | **0.93**      | **0.92**   | **0.93**     | **0.984**   | Best for high-precision applications requiring robust performance.                             |
| Gradient Boost Classifier       | 0.91          | 0.88       | 0.89         | 0.971       | Effective for imbalanced datasets.                                                             |
| Support Vector Machines (SVM)   | 0.88          | 0.84       | 0.86         | 0.950       | Suitable for smaller datasets with clear separable classes.                                    |
| Linear Regression               | 0.87          | 0.83       | 0.85         | 0.946       | Basic predictions where linear relationships dominate.                                         |


---

## 🌐 Applications
- **Clinical Diagnostics**:
  - Rapid identification of high-risk bacterial strains.
- **Therapeutic Development**:
  - Targeting virulence factors for personalized treatments.
- **Public Health**:
  - Understanding pathogen evolution for epidemic preparedness.

---

## 📚 References
1. **L. Brierley et al.,** *Tissue tropism and transmission ecology predict virulence of human RNA viruses.* [DOI Link](https://doi.org/10.1371/journal.pbio.3000206)
2. **C. Bonneaud & B. Longdon,** *Emerging pathogen evolution.* [DOI Link](https://doi.org/10.15252/embr.202051374)

---


