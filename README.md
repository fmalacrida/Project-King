Machine Learning Project: Housing Price Analysis in King County

Project Overview

This project focuses on analyzing and predicting housing prices using various machine learning techniques. The dataset contains features such as price, number of bedrooms and bathrooms, square footage, and location (ZIP code, latitude, longitude). The project explores the data, preprocesses it, and builds predictive models to estimate house prices.

Steps and Decisions Made

1. Data Extraction
	•	The dataset was loaded using pandas.
	•	A utility function was defined to standardize column names to snake_case for consistency.
	•	Initial exploration was conducted to understand the dataset’s shape, data types, and random samples.

2. Data Cleaning and EDA
	•	Duplicates and Missing Values: Checked for duplicate rows, NaN values, and empty spaces.
	•	Outliers: Boxplots were used to identify and assess potential outliers in numerical features like price, sqft_living, and sqft_lot.

3. Feature Engineering
	•	Feature Transformation:
	•	Created five new features to split condition feature levels.
	•	Encoded categorical features like ZIP codes into meaningful clusters.
	•	Feature Importance:
	•	Assessed the importance of features like zip code, latitude, and longitude, deciding whether to combine or retain them individually.

4. Data Splitting
	•	The dataset was split into features (X) and target (y), ensuring the target variable (price) was correctly excluded from the feature set.

5. Model Building
	•	Various machine learning models were trained and evaluated:
	•	Linear Regression
	•	Ridge and Lasso Regression
	•	Random Forest Regressor
	•	XGBoost Regressor
	•	Model performance was assessed using metrics like Mean Squared Error (MSE) and R-squared.

6. Model Evaluation and Selection
	•	Used cross-validation to evaluate the models and mitigate overfitting.
	•	Chose the best-performing model based on evaluation metrics: XGBoost Regressor

7. Visualization
	•	Histograms:
			Analyzed distributions of key features (price, sqft_living, etc.).
	•	Boxplots:
			Visualized outliers and distributions for numerical features.
			Geographical Maps:
			Created maps with Folium to explore geographical data, leveraging latitude and longitude.

8. Conclusion
	•	The final model provided accurate predictions for housing prices.
	•	Insights from feature importance and clustering were used to recommend data-driven strategies for decision-making in real estate.

Files in the Repository
	•	Notebook: The full implementation of the project.
	•	Dataset: The CSV file used in this analysis (ensure data privacy and integrity if sharing publicly).
	•	README: Documentation of the project (this file).