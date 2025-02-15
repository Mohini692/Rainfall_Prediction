#Rainfall Prediction using Machine Learning 

🚀 Project Overview
This project aims to predict whether rainfall will occur based on various meteorological features. Using machine learning techniques, we classify rainfall occurrence as:
✅ Yes (1) – Rainfall will happen
❌ No (0) – No Rainfall

📊 Dataset Description
The dataset consists of various meteorological attributes, including:

🌡 Temperature (Max, Min, Avg)
💨 Wind Speed & Direction
🌥 Cloud Cover & Sunshine Duration
🌡 Dew Point & Humidity
⏬ Pressure
☔ Rainfall (Target Variable: 1 = Rain, 0 = No Rain)

🔍 Exploratory Data Analysis (EDA)
✅ Data Cleaning:
Stripped column names for consistency.
Dropped unnecessary columns (day).
Imputed missing values using median imputation for wind direction and wind speed.

✅ Data Visualization:
📊 Histograms for numerical feature distributions.
📉 Boxplots to detect outliers.
🔥 Correlation Heatmap to analyze feature relationships.

🛠 Feature Engineering & Preprocessing
Converted categorical target:
"Yes" → 1
"No" → 0
Removed highly correlated features: maxtemp, dewpoint, mintemp
Balanced the dataset using downsampling to address class imbalance.

📌 Train-Test Split:
80% Training
20% Testing

🤖 Model Development
✅ Random Forest Classifier was used for classification.
✅ Hyperparameter Tuning with GridSearchCV:

🌳 n_estimators: [50, 100, 200]
🔢 max_features: ["sqrt", "log2"]
📏 max_depth: [None, 10, 20, 30]
🏗 min_samples_split: [2, 5, 10]
🍂 min_samples_leaf: [1, 2, 4]
✅ Cross-Validation applied to enhance model stability.
📈 Model Evaluation
📌 Test Set Accuracy: ✅ High performance achieved.
📌 Metrics Used:

📊 Confusion Matrix
📑 Classification Report (Precision, Recall, F1-score)
📉 Cross-validation scores

Conclusion & Future Work
✔ Random Forest Classifier performed well in predicting rainfall.
✔ Feature selection & class balancing improved the model's performance.

 Future Enhancements:
📊 More Feature Engineering for better predictive power.
🧠 Ensemble Learning to further boost accuracy.
