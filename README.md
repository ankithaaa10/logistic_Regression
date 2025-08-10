Binary Classification with Logistic Regression (Breast Cancer Dataset)


This repo implements a **binary classification model** using **Logistic Regression** on the **Breast Cancer Wisconsin dataset**.  
The goal is to classify tumors as **Malignant** or **Benign** based on 30 numerical features from digitized medical images.

---

## 📂 Dataset
- **Source**: Built-in dataset from scikit-learn
- **Samples**: 569
- **Features**: 30 numerical variables (e.g., radius, texture, smoothness, symmetry)
- **Target**:
  - 0 → Malignant (cancerous)
  - 1 → Benign (non-cancerous)

---

## ⚙️ Steps Performed
1. **Data Loading**
   - Used load_breast_cancer() from scikit-learn.
   - Converted data into a Pandas DataFrame.

2. **Train/Test Split**
   - 80% training, 20% testing.

3. **Feature Scaling**
   - Standardized features using StandardScaler for better model convergence.

4. **Model Training**
   - Trained a **Logistic Regression** model with max_iter=5000.

5. **Evaluation**
   - **Confusion Matrix** (True Positives, True Negatives, False Positives, False Negatives)
   - **Classification Report**: Precision, Recall, F1-score
   - **ROC Curve** and **AUC Score**

6. **Threshold Tuning**
   - Adjusted probability cutoff from 0.5 to 0.4 and analyzed impact on predictions.

7. **Sigmoid Function**
   - Plotted the **sigmoid curve** to understand probability mapping in logistic regression.

---

## 📊 Model Performance (Example Output)
| Metric       | Value |
|--------------|-------|
| Accuracy     | 97%   |
| Precision    | 97%   |
| Recall       | 98%   |
| ROC-AUC      | 0.99  |



---

## 📈 Visualizations
- Confusion Matrix (default threshold)
- ROC Curve with AUC
- Confusion Matrix after threshold tuning
- Sigmoid Function plot
