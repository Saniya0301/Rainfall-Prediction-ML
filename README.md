🌧️ Rainfall Prediction ML Project


Overview

This project demonstrates building a rainfall prediction model using historical weather data, preprocessing, exploratory analysis, training a Random Forest classifier, followed by evaluation and visualization.

🚀 Getting Started
Dataset Loading & Cleaning
Load rainfall.csv using pandas.

Strip and rename columns to remove trailing spaces.

Impute missing values (e.g., mean imputation for wind direction/speed).

Convert categorical labels (‘yes’/’no’) to numeric 1/0.


Exploratory Data Analysis (EDA)
Visualize distributions for numerical features (pressure, dew point, humidity, etc.).

Plot correlations and heatmaps.

Observe relationships such as higher humidity and dew point signaling rainfall days—mirroring real-world behavior 

.

Feature Engineering
Drop redundant features (e.g. max and min temperature if highly correlated).

Separate features and target label.

Handling Class Imbalance
Use RandomOverSampler to balance minority ‘rain’ class before training 


Model Training
Split data into training and validation sets.

Train various classifiers: Logistic Regression, XGBoost, SVC, and Random Forest.

Random Forest is used in the video walkthrough.

Evaluation
Compute ROC-AUC score on both train and validation sets.

## 🧠 Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Imbalanced-learn (`RandomOverSampler`)
- Jupyter Notebook

## 📊 Exploratory Data Analysis (EDA)

Key insights from the EDA include:
- Strong correlation between humidity, dew point, and rainfall
- Visual analysis through heatmaps, histograms, and pair plots
- Removal of redundant or highly correlated features

- Trained multiple ML algorithms:
- Logistic Regression
- SVC (Support Vector Classifier)
- Random Forest (Best performing)
- XGBoost (optional)

**Class Imbalance Handling**: Applied `RandomOverSampler` to balance the dataset due to fewer rainy days.

**Evaluation Metrics**:
- Accuracy
- Precision, Recall, F1-score
- Confusion Matrix
- ROC-AUC Score

---
📈 Sample Output
Accuracy: ~85%

Recall (Rainy class): ~94%

ROC-AUC Score: 0.87

Confusion matrix and classification reports are displayed in the notebook.

📌 Future Improvements
Hyperparameter tuning (GridSearchCV)

Use time-series models (like LSTM or ConvLSTM)

Deploy the model using Flask or Streamlit

Integrate external live weather APIs


🙋‍♀️ About Me

Hi, I'm Saniya Chhabra – a tech enthusiast learning and building practical ML projects.
Let's connect on LinkedIn or collaborate on more ML/AI projects! 💡



📄 License
This project is open-source and available under the MIT License.

