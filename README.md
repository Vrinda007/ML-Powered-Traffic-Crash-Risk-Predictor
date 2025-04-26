This project, **"Analyzing and Predicting Traffic Accident Severity Using Machine Learning"**, presents a practical, data-driven solution for predicting the severity of car accidents. Using a robust **Logistic Regression model**, I developed a predictive pipeline that classifies crash incidents into two categories: **"No Injury / Drive Away"** and **"Injury and/or Tow Due to Crash"**.

The project addresses critical real-world challenges such as emergency service planning, urban traffic safety management, and insurance risk assessment. Emphasis was placed on ethical model development, including tackling data imbalance, ensuring model interpretability, and mitigating biases.

---

## Project Goals
- Build an **interpretable and efficient Logistic Regression model** for binary crash severity classification.
- Handle **class imbalance** using balanced class weighting and fair evaluation metrics.
- Maintain **high model transparency** for ethical deployment and real-world applicability.
- Deliver **practical business value** for emergency services, insurance companies, and traffic authorities.

---

## Technologies Used
- **Python** (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- **Machine Learning**: Logistic Regression (with balanced class weights)
- **Data Analysis**: Exploratory Data Analysis (EDA), feature engineering, outlier handling
- **Visualization**: Heatmaps, correlation matrices, boxplots, ROC and Precision-Recall curves

---

## Key Deliverables

### 1. Data Preparation
- Imported real-world crash data from Kaggle.
- Conducted initial data inspection and statistical summaries.
- Performed outlier detection and removal using **Interquartile Range (IQR)** method.
- Engineered features such as `Crash Hour`, `Weekday`, and `Is_Weekend`.
- Encoded categorical variables with **Label Encoding** while maintaining interpretability.

### 2. Exploratory Data Analysis (EDA)
- Generated insights into crash trends by hour, day, and month.
- Analyzed correlations between weather, road type, lighting conditions, and accident severity.
- Identified key accident-prone periods and environmental conditions.

### 3. Model Development
- Built a **Logistic Regression** model with:
  - Balanced class weights to address severe data imbalance.
  - `Linear` solver for computational efficiency.
- Split dataset into **Training (80%)** and **Testing (20%)** sets.
- Ensured reproducibility with fixed random states.

### 4. Model Evaluation
- Achieved **Accuracy**: 79.27%
- **Precision**: 75.51% | **Recall**: 79.33% | **F1-Score** (for severe crashes): 0.88
- **Precision-Recall AUC**: 0.9183, indicating high robustness against class imbalance.
- Visualized model performance using:
  - Confusion Matrix
  - ROC Curve
  - Precision-Recall Curve
  - Predicted vs. Actual comparison plots

---

## Business Value
- **Emergency Services**: Early identification of accident hotspots enables better ambulance/resource allocation.
- **Insurance Industry**: Supports fairer risk assessments and faster claim evaluations.
- **Urban Traffic Authorities**: Enables targeted interventions in high-risk zones based on crash severity forecasts.

Despite minor limitations such as difficulty predicting rare non-severe cases due to dataset imbalance, the model demonstrates strong potential for real-world deployment where **accuracy**, **recall**, and **interpretability** are mission-critical.

---

## Ethical Considerations
- **Bias Mitigation**: Accounted for data imbalance and transparent feature encoding.
- **Model Interpretability**: Ensured conclusions remain correlational rather than causational.
- **Deployment Safeguards**: Proposed monitoring systems and impact audits for responsible real-world deployment.

---

## Future Improvements
- Integrate contextual variables like **driver behavior** and **traffic density**.
- Explore **hybrid models** that combine Logistic Regression interpretability with ensemble model performance.
- Strengthen minority class predictions using advanced sampling techniques like SMOTE.

---
Thank you for visiting! 
