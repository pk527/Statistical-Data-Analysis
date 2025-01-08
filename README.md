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

 
## Methodology
The research follows these steps:

1. **Data Collection**: Bacterial pathogens and their ecological features were compiled from public datasets.
2. **Feature Engineering**: Focused on key factors such as:
   - Transmissibility
   - Tissue Tropism
   - Severity
3. **Model Development**: Used classification algorithms to predict virulence:
   - Random Forest
   - Gradient Boosting
   - Logistic Regression
4. **Evaluation**: Models were assessed using metrics such as accuracy, precision, recall, F1-score, and ROC-AUC.
5. **Visualization**: SHAP, LIME, and other techniques were employed for interpretability.

## Results
### Key Findings
1. **Feature Importance**:
   - The most significant predictors of bacterial virulence are:
     - **Tissue Tropism**: Pathogens with neural or renal tropism have higher virulence.
     - **Transmissibility**: Pathogens with limited person-to-person transmission are more likely to cause severe disease.
     - **Severity Scale**: Measures the potential impact of pathogens on human health.
2. **Model Performance**:
   - The **Random Forest Classifier** achieved the best performance among all tested models, demonstrating:
     - **Accuracy**: 94.5%
     - **Precision**: 92.3%
     - **Recall**: 93.7%
     - **F1-Score**: 93.0%
     - **ROC-AUC**: 0.92
   - This model was chosen for its balance of high precision and recall, ensuring robust predictions for high-virulence pathogens.

### Model Selection
The **Random Forest Classifier** was selected as the final model due to its superior performance metrics and interpretability. Compared to other models (e.g., Gradient Boosting and Logistic Regression), Random Forest consistently provided:
- Higher accuracy and AUC scores.
- Greater flexibility in handling categorical and continuous variables.
- Better feature importance insights for ecological factors driving predictions.


   ## 📈 Results and Insights
| **Model**                       | **Precision** | **Recall** | **F1 Score** | **AUC-ROC** | **Best Use Case**                                                                                  |
|---------------------------------|---------------|------------|--------------|-------------|-----------------------------------------------------------------------------------------------|
| Random Forest Classifier        | **0.93**      | **0.92**   | **0.93**     | **0.984**   | Best for high-precision applications requiring robust performance.                             |
| Gradient Boost Classifier       | 0.91          | 0.88       | 0.89         | 0.971       | Effective for imbalanced datasets.                                                             |
| Support Vector Machines (SVM)   | 0.88          | 0.84       | 0.86         | 0.950       | Suitable for smaller datasets with clear separable classes.                                    |
| Linear Regression               | 0.87          | 0.83       | 0.85         | 0.946       | Basic predictions where linear relationships dominate.                                         |

### **3. Interactive Visualizations**

1. **SHAP Summary Plot**
   - **Purpose**: Displays the global importance of features in predicting bacterial virulence.
   - **Details**: The SHAP summary plot ranks features by their average absolute SHAP value, visually depicting the impact of each feature on the model's predictions.
   - **Example**: Tissue tropism and transmissibility emerge as the most influential features, with their corresponding SHAP values distributed across predictions.
   - **Interpretation**: The plot enables users to quickly identify which features contribute the most to the predictions.

2. **ROC-AUC Curve**
   - **Purpose**: Evaluates the trade-off between sensitivity (True Positive Rate) and specificity (False Positive Rate).
   - **Details**: The Receiver Operating Characteristic (ROC) curve plots TPR vs. FPR for different classification thresholds.
   - **Example**: An AUC of 0.92 indicates a high-performing model with excellent discriminative ability.
   - **Interactive Element**: The curve allows users to understand how adjusting thresholds impacts the model's ability to balance false positives and false negatives.

3. **Feature Importance Plot**
   - **Purpose**: Highlights the ranked importance of features in the machine learning model.
   - **Details**: Bar plots display the relative importance scores assigned to features based on their contribution to predictive accuracy.
   - **Example**: Features like transmissibility and severity score receive the highest importance, corroborating the findings from SHAP.
   - **Visualization Benefits**: Simplifies feature prioritization for domain-specific interventions.

4. **LIME Explanations**
   - **Purpose**: Provides interpretability for individual predictions by showing how feature values influenced the outcome.
   - **Details**: The Local Interpretable Model-Agnostic Explanations (LIME) output visualizes feature contributions for a single sample.
   - **Example**: For a high-virulence prediction, LIME highlights key factors such as neural tropism and low transmissibility.
   - **Interactive Insight**: LIME enables researchers to validate and challenge predictions on a case-by-case basis, ensuring robust decision-making.



---

## 🔍 Analytical Questions Explored
1. **What ecological and transmission factors strongly influence bacterial pathogen virulence?**
2. **How does tissue tropism correlate with severity levels?**
3. **What model provides the best prediction accuracy, and why?**
4. **How do upsampling and feature encoding improve model performance?**
5. **Which pathogens are misclassified, and what are the reasons?**

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


