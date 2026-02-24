# MLOps: Automated Model Lifecycle & Pipeline Integrity

### *Ensuring Statistical Reliability and Production Stability in ML Workflows*

## 📌 Project Overview
As a Data Scientist, my goal is to bridge the gap between a "working notebook" and a "reliable production system." This repository demonstrates a complete MLOps pipeline that automates the testing, versioning, and deployment of Machine Learning models.

By utilizing GitHub Actions and Azure ML, this project ensures that every model update undergoes rigorous validation before deployment, minimizing "silent failures" in production environments.

It on the end-to-end automation of a **Random Forest Regression** model designed to predict asset prices (specifically used cars). In a manufacturing context, this architecture is directly applicable to **Predictive Maintenance Costing** and **Procurement Optimization**.

The repository demonstrates a transition from exploratory data analysis to a robust **CI/CD pipeline** using **GitHub Actions** and **Azure**, ensuring that the regression model remains accurate and deployable.

## 🚀 Data Science & Regression Capabilities
* **Model Architecture:** Implemented a **Random Forest Regressor**, leveraging ensemble learning to handle non-linear relationships and reduce overfitting.
* **Feature Engineering:** Meticulous data preprocessing, including handling categorical variables and scaling numerical features to improve model convergence.
* **Hyperparameter Tuning:** Optimized the Forest's depth and estimator count to balance bias and variance.
* **Automated Validation:** Every code push triggers a suite of tests that check for data drift and verify that the model's $R^2$ score meets production standards.
* **Environment Consistency:** Use of Docker and Conda environments to guarantee reproducibility across development, staging, and production.
* **Cloud Orchestration:** Automated deployment to Azure Machine Learning for scalable model hosting and inference.

<img width="1437" height="436" alt="image" src="https://github.com/user-attachments/assets/7f912d35-cc17-480d-9bd7-49412bc77c66" /> 

 Source: [Actions Page](https://github.com/varuni-rao/Random-Forest-Regression-Pipeline/actions/runs/13973767090)

## 🧪 Experimentation & Research
The core logic was developed in the **Used Car Price Prediction** notebook, focusing on statistical validation:
* **Exploratory Data Analysis (EDA):** Identified key price drivers such as mileage, age, and fuel type.
* **Performance Metrics:** Evaluated the model using Mean Absolute Error (MAE) and $R^2$ to ensure high prediction confidence.
* **Live View:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/varuni-rao/Github-Actions-CI-CD/blob/main/notebooks/MLOps_Regression_Pipeline.ipynb)

## 🛠 Technical Stack
* **Frameworks:** Scikit-Learn, Pandas, NumPy
* **Orchestration:** GitHub Actions (CI/CD)
* **Cloud:** Microsoft Azure (Azure ML SDK)
* **Visualization:** Matplotlib, Seaborn

## 📂 Repository Structure
.github/workflows/: YAML definitions for the automated Data Science pipeline.
src/: Core Python modules for data preprocessing, training, and evaluation.
tests/: Statistical and functional tests to ensure model integrity.
notebooks/: Notebook used to create the source files and display the pipeline run results on Azure
requirements.txt: Strict dependency management for reproducibility.

## 🏭 The Industrial Parallel: Control Systems & MLOps
My background as a **SCADA Engineer at ABB** (MicroSCADA for Tata Power) directly informs my MLOps strategy:

* **Signal Integrity:** Just as a SCADA system relies on accurate sensor data, this regression pipeline includes data validation steps to ensure "garbage in" doesn't lead to "garbage out."
* **Redundancy:** Similar to redundant control loops in power grids, the Random Forest ensemble provides a "majority vote" system that is more resilient than single-tree models.
* **Operational Monitoring:** I treat the ML model's $R^2$ score like a critical system parameter—if it deviates from the setpoint, the pipeline triggers an alert for manual review.

---

## 🔧 Installation & Usage
1. **Clone:** `git clone https://github.com/varuni-rao/Github-Actions-CI-CD.git`
2. **Setup Secrets:** Add `AZURE_CREDENTIALS` to your GitHub repository secrets.
3. **Trigger:** Push a change to `src/` to start the automated Regression workflow.

