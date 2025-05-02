🎧 Regression Model: Predicting Podcast Listening Time

📈 Project Overview

This project focuses on developing a regression model to predict the expected listening time of a podcast episode. We explore different algorithms to understand and generalize which features (such as podcast title, episode length, number of ads, episode number, etc.) most influence a user's likelihood of listening.

🧰 Tools Used

* Python & Pandas – For data cleaning and manipulation
* Scikit-learn – For encoding categorical variables, scaling numerical features, and building various regression models
* Matplotlib & Seaborn – For visualization and exploratory data analysis

🔎 Exploratory Data Analysis & Cleaning

* Employed matplotlib and seaborn to examine relationships between input features and the target variable
* Used histograms, density plots, and bar charts to explore the distribution of numerical features
* Imputed missing values using pandas and scikit-learn techniques
* Corrected anomalous data based on its correlation with the target variable

🧱 Feature Engineering

* Created new features by combining existing columns
* Evaluated how these engineered features impacted the model’s predictive power

🧪 Data Normalization

* Split the dataset into training, validation, and test sets using train_test_split
* Applied one-hot encoding to categorical variables via OneHotEncoder
* Scaled numerical features using MinMaxScaler

🧮 Model Development

* Built baseline models (mean and median predictors) to serve as performance benchmarks
* Experimented with linear models including LinearRegression, Ridge, and Lasso
* Leveraged tree-based models like XGBRegressor and RandomForestRegressor
* Tuned hyperparameters using RandomizedSearchCV for optimal performance
* Developed a custom ensemble class to combine tree-based and linear models

✨ Key Insights

* After evaluating model performance using RMSE, we selected a tuned XGBRegressor and a basic LinearRegression model
* These were ensembled with weights of 0.8 (XGB) and 0.2 (Linear), achieving an RMSE of 12.70 on the validation set, and 12.84 on Kaggle's test set
* Our final model ranked within the top 25% of all participants in the Kaggle competition

📂 How to Run the Project

* Download the dataset from the link below
* Update the file path in the Jupyter Notebooks
* Run the notebook to reproduce the results

🔗 Dataset: https://www.kaggle.com/competitions/playground-series-s5e4
