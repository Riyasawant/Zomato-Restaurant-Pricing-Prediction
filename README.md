# Zomato-Restaurant-Pricing-Prediction
**Introduction**
This report presents an analysis of restaurant pricing prediction using machine learning models. The goal is to predict the approximate cost for two people at a restaurant based on various features such as location, cuisine, and restaurant type. The dataset used for this analysis is sourced from Zomato, a popular restaurant discovery and food delivery platform.

**Data Overview:**
The dataset contains information about restaurants listed on Zomato. 
Key features include:Restaurant Name: The name of the restaurant.Location: The geographic area where the restaurant is located.Cuisines: Types of cuisines served.Average Cost for Two: The target variable, representing the approximate cost for two people.Rating: The average rating given by customers.Votes: Number of votes received.Online Order: Indicates if the restaurant accepts online orders (Yes/No).Book Table: Indicates if the restaurant offers table booking (Yes/No).Restaurant Type: Type of restaurant (e.g., Casual Dining, Café).

**Data Preprocessing**
Handling Missing Values: First, we check for missing values in the dataset and handle them appropriately. Missing values in categorical columns are filled with the mode, while missing values in numerical columns are filled with the median.Encoding Categorical VariablesCategorical variables such as Location, Cuisines, Online Order, Book Table, and Restaurant Type are encoded using label encoding and one-hot encoding techniques.Feature EngineeringNew features are created to capture interactions between existing features. For instance, we create a feature that combines Location and Restaurant Type to capture location-specific restaurant types.Normalizing Numerical FeaturesNumerical features such as Votes and Rating are normalized using standard scaling to ensure that they have a mean of zero and a standard deviation of one.

Exploratory Data Analysis (EDA)Correlation Analysis: A correlation matrix is generated to identify relationships between features and the target variable. Highly correlated features are noted for further analysis.VisualizationVarious visualizations such as bar plots, pie charts, and heatmaps are used to explore the distribution of features and their relationship with the target variable.

**Model Building**
Train-Test Split: The dataset is split into training and testing sets using an 80-20 split to ensure that the models are evaluated on unseen data.Baseline ModelA baseline model using linear regression is built to provide a benchmark for evaluating other models.
Advanced Models: Several machine learning models are implemented and evaluated, including:
  1. Random Forest Regressor: An ensemble model that uses multiple decision trees to improve predictive performance.
  2. XGBoost Regressor: A gradient boosting model that is highly effective for structured data.
  3. K-Nearest Neighbors (KNN): A non-parametric method that predicts the target by averaging the nearest neighbors.
  4. AdaBoost Regressor: An ensemble model that combines multiple weak learners to create a strong learner.
  5. Decision Tree Regressor: A simple decision tree model that splits the data based on feature values.

**Model Evaluation**
Models are evaluated using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²) score. Cross-validation is performed to ensure that the models generalize well to unseen data.
![image](https://github.com/Riyasawant/Zomato-Restaurant-Pricing-Prediction/assets/66208299/63789f1e-013f-41fa-b649-e06909ffa900)


**Results**
Model PerformanceThe performance of each model is compared based on the evaluation metrics. The model with the best performance is selected as the final model for predicting restaurant prices. The best model is XGBoost Regression giving accuracy of 98%.
