# Engine Sentinel – Predictive Maintenance for Aerospace Engines ✈️

## Overview
Engine Sentinel is a machine learning-based predictive maintenance system designed to estimate the **Remaining Useful Life (RUL)** of aerospace turbofan engines. Using NASA's **CMAPSS Turbofan Engine Degradation Simulation Dataset**, this project builds a robust Gradient Boosted Trees model that enables **proactive maintenance**, reducing downtime, enhancing safety, and optimizing resources.

## 🔍 Project Objectives
- Predict RUL of turbofan engines using sensor data.
- Compare and evaluate machine learning models including **Gradient Boosted Trees** and **Random Forest**.
- Build a scalable and reliable model suitable for deployment in real-world aerospace scenarios.

## 📊 Dataset
- **Source**: NASA Ames Prognostics Data Repository  
- **Dataset**: [CMAPSS Jet Engine Simulated Data](https://data.nasa.gov/Aeorspace/CMAPSS-Jet-Engine-Simulated-Data/ff5v-kuh6)
- **Subsets**: FD001, FD002, FD003, FD004 – varying by fault modes and operational conditions

## 🧪 Methodology
1. **Data Preprocessing**
   - Normalization
   - Anomaly Detection
   - Handling missing values

2. **Feature Engineering**
   - Trend extraction
   - Statistical summaries (mean, variance, slope)
   - Domain-specific indicators

3. **Modeling**
   - Models used: `Random Forest`, `Gradient Boosted Trees (XGBoost)`
   - Cross-validation for robust performance
   - Hyperparameter tuning

4. **Evaluation**
   - Metric: Normalized Root Mean Square Error (RMSE)
   - Visualization: Box plots, bar graphs of risk levels

## ✅ Results
| Dataset | Model              | Normalized RMSE |
|---------|--------------------|------------------|
| FD001   | Gradient Boosted Trees | **1.54%**         |
| FD002   | Gradient Boosted Trees | **1.89%**         |
| FD003   | Gradient Boosted Trees | **1.57%**         |
| FD004   | Gradient Boosted Trees | **1.98%**         |

- **Gradient Boosted Trees outperformed** Random Forests in all datasets.
- Risk level classification provided actionable maintenance insights.

## 💻 Tech Stack
- Python 3.9
- Libraries: `pandas`, `numpy`, `scikit-learn`, `xgboost`, `matplotlib`
- Environment: Jupyter Notebook
- Hardware: Intel Core i7, 16 GB RAM

## 📈 Visual Outputs
- RMSE comparison charts
- Risk level bar graphs
- RUL distribution box plots
- CSV outputs with engine-specific RUL predictions

## 📌 Conclusion
Engine Sentinel demonstrates the power of predictive analytics in aerospace maintenance. With high accuracy and scalability, this model can enhance operational safety and significantly reduce unplanned engine failures.

## 🔮 Future Work
- Real-time deployment of RUL prediction system
- Incorporate deep learning models (e.g., LSTM, CNN)
- Expand feature sets with external environmental and flight data

## 👨‍💻 Author
**Sasi Praneeth Reddy Sadhu**  
Graduate Student, George Mason University  
📧 ssadhu2@gmu.edu

## 📚 References
1. [Predictive maintenance advances - IEEE](https://ieeexplore.ieee.org/document/8666136)  
2. [NASA CMAPSS Dataset](https://data.nasa.gov/Aeorspace/CMAPSS-Jet-Engine-Simulated-Data/ff5v-kuh6)  
3. [Gradient Boosting Intro - Machine Learning Mastery](https://machinelearningmastery.com/gentle-introduction-gradient-boosting-algorithm-machine-learning/)
