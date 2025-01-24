# IIT-KGP-data-analytics-hackathon
# 🌟 NSSC Hackathon Project: Cosmic Collision-Analysing Asteroid Risks with Data

## 📝 Problem Statement
The primary objective of this analysis is to use data analytics and machine learning techniques
to determine the likelihood of an asteroid being hazardous to Earth based on various features
provided in the dataset. This includes examining characteristics such as the asteroid's size,
orbital parameters, velocity, and proximity to Earth's orbit.

The dataset contained values of different features eg epoch osculation, relative velocity, aphelion distance etc. Our goal was to not only build an accurate model but also ensure it was interpretable and efficient.

---

## 💡 Solution Overview
To address the problem effectively, we employed the **Random Forest Algorithm**, a powerful ensemble learning method known for:
- Handling large datasets with higher dimensionality.
- Mitigating overfitting through bagging and random feature selection.
- Offering feature importance insights for better interpretability.

### **Approach Breakdown**
1. **Data Exploration and Preprocessing**:
   - Analyzed the dataset to identify trends, missing values, and potential outliers.
   - Cleaned and transformed the data by:
     - Handling missing values appropriately.
     - Encoding categorical variables.
     - Normalizing or standardizing numerical features as needed.

2. **Feature Selection**:
   - Leveraged Random Forest’s inbuilt feature importance mechanism to identify critical features.
   - Reduced redundant or irrelevant features to enhance model performance.

3. **Model Development**:
   - Used `RandomForestClassifier` (or `RandomForestRegressor`) from Scikit-learn.
   - Tuned hyperparameters such as:
     - Number of trees (`n_estimators`).
     - Maximum depth of trees (`max_depth`).
     - Minimum samples split (`min_samples_split`).
   - Applied cross-validation to validate the model's robustness.

4. **Evaluation and Insights**:
   - Evaluated the model using metrics like:
     - Classification tasks: Accuracy, F1-Score, and Confusion Matrix.
     - Regression tasks: Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² score.
   - Visualized feature importance and other insights using Matplotlib and Seaborn.

---

## 📊 Results
Our Random Forest model demonstrated:
- **Accuracy**: 83% on the test set.
- Significant insights into feature importance, highlighting [kMiles per hour].

These results validated the robustness of our approach and showcased its scalability for real-world applications.

---

## 🔧 Tools and Technologies
- **Programming Language**: Python
- **Key Libraries**: 
  - Scikit-learn
  - Pandas
  - NumPy
  - Matplotlib & Seaborn (visualization)
  - [Optional: Flask/Streamlit for deployment]

---
