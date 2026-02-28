# Breast Cancer Detection Using Logistic Regression

## Project Overview
This project uses **Logistic Regression** to build a machine learning model that predicts whether a given breast cancer cell is **malignant** or **benign** based on various features extracted from digitized images of breast cancer cells. The model is trained using the **Breast Cancer dataset**, which includes detailed measurements of cell attributes.

## Objective
The objective of this project is to apply machine learning techniques to train a logistic regression model capable of predicting the malignancy of breast cancer cells based on their features. The goal is to accurately classify whether a cell is malignant (cancerous) or benign (non-cancerous), thus aiding in early detection and diagnosis of breast cancer.

## Dataset
The project utilizes the **Breast Cancer dataset** (available from UCI's Machine Learning Repository), which contains the following attributes:
- **Radius**: Mean of distances from center to points on the perimeter.
- **Texture**: Standard deviation of gray-scale values.
- **Perimeter**: Perimeter of the tumor.
- **Area**: Area of the tumor.
- **Smoothness**: Local variation in radius lengths.
- **Compactness**: Perimeter^2 / Area - 1.0
- **Concavity**: Severity of concave portions of the contour.
- **Concave points**: Number of concave portions of the contour.
- **Symmetry**: Symmetry of the tumor.
- **Fractal Dimension**: Coastline approximation - describes the complexity of the tumor.

The target variable, **diagnosis**, indicates whether a tumor is malignant (`M`) or benign (`B`).

## Steps Involved

1. **Data Preprocessing:**
   - Cleaned and prepared the dataset by dropping irrelevant columns.
   - Handled missing values and scaled numerical features using **MinMaxScaler**.
   - Converted the target variable (`diagnosis`) into a binary format (1 for malignant, 0 for benign).

2. **Exploratory Data Analysis (EDA):**
   - Explored the data using statistical summaries and visualizations bargraph and heatmap to review the data better.
   - Visualized the distribution of the target variable

3. **Model Training:**
   - Trained a **Logistic Regression** model to classify breast cancer cells as malignant or benign.
   - Split the dataset into training and testing sets, with **80%** used for training and **20%** for testing.

4. **Model Evaluation:**
   - Evaluated the model using various metrics such as:
     - **Accuracy**: The proportion of correct predictions.
     - **Confusion Matrix**: The matrix showing true positives, false positives, true negatives, and false negatives.
     - **Classification Report**: Metrics like precision, recall, and F1-score for each class (malignant and benign).

## Key Results
- **Training Accuracy**: 97%
- **Test Accuracy**: 98%
- **Confusion Matrix**:
  - **Training**: [[285   1], [13 156]]
  - **Test**: [[71 0], [2 41]]
- **Classification Report**:
  - High precision, recall, and F1-score for both malignant and benign classes.
  - The model achieved an overall **accuracy of 97%** on the training set and **98%** on the test set.

## Insights
- The logistic regression model is highly accurate in predicting the malignancy of breast cancer cells, with minimal false positives and false negatives.
- The high precision and recall values indicate that the model is effective in distinguishing between benign and malignant cells, which is crucial in medical diagnostics.
