
# DSN-MICROSOFT-HACKATHON 

## Wazobia Real Estate Limited House Price Prediction: 1st Place Solution

## Description
Welcome to the Wazobia Real Estate Limited Predictive Modeling Hackathon! This exciting data science competition is dedicated to the accurate prediction of house prices in Nigeria. Our mission is to collaboratively develop powerful predictive models that empower Wazobia Real Estate with the insights they need to make informed pricing decisions and excel in the competitive real estate market.

### Goal
The primary objective of this hackathon is to create a robust predictive model that can accurately estimate house prices in Nigeria. By harnessing the potential of the provided dataset, participants will craft sophisticated models that generate dependable price predictions for Wazobia Real Estate's diverse properties.

### Objectives
- Data Analysis: Delve into the dataset through comprehensive exploratory data analysis. Identify outliers, tackle missing values, and gain a deep understanding of the data's underlying characteristics.

- Model Building: Employ advanced machine learning algorithms to construct predictive models. Strive for models that offer exceptional accuracy in forecasting house prices.

- Model Evaluation: Rigorously evaluate model performance using appropriate metrics. Through meticulous evaluation, select the most effective and precise predictive model.

- Interpretability: Unearth the influential factors that shape house prices. Interpret the model results to gain valuable insights into the dynamics of the real estate market.

- Business Impact: Translate model insights into actionable strategies that can transform Wazobia Real Estate's pricing tactics and enhance their competitive edge.





## Installation

To get started with the Wazobia Real Estate Predictive Modeling Hackathon, follow these installation steps:

1. **Clone the Repository:** Begin by cloning this repository to your local machine using the following command:

    ```bash
    git clone https://github.com/FelixFrankFelix/DSN-MICROSOFT-HACKATHON.git
    ```

2. **Navigate to the Directory:** Move into the project directory:

    ```bash
    cd DSN-MICROSOFT-HACKATHON
    ```

3. **Create a Virtual Environment (Optional):** While not mandatory, it's recommended to create a virtual environment to isolate the project dependencies. You can create a virtual environment using `venv` or `conda`. For `venv`, execute:

    ```bash
    python -m venv venv
    ```

    Activate the virtual environment:

    - On Windows:
      ```bash
      venv\Scripts\activate
      ```
    - On macOS and Linux:
      ```bash
      source venv/bin/activate
      ```

4. **Install Dependencies:** Install the required Python packages using `pip`:

    ```bash
    pip install pandas numpy scikit-learn catboost seaborn matplotlib

    ```

5. **Run the Jupyter Notebook:** Launch the Jupyter Notebook to explore the provided dataset and participate in the hackathon:

    ```bash
    jupyter notebook
    ```

6. **Open the Notebook:** In your web browser, navigate to `http://localhost:8888` to access the Jupyter Notebook interface. Open the `Exploratory Data Analysis.ipynb` notebook to get insight about the data, then `Data Preprocessing-Modelling.ipynb` notebook to start your data transformation and model building journey.

That's it! You're all set to dive into the Wazobia Real Estate Predictive Modeling Hackathon. Happy coding and data exploring!


## Data Description and EDA

This dataset contains valuable information on various features related to houses, including the number of bathrooms, bedrooms, parking spaces, property types, and their corresponding prices. The goal of this hackathon is to develop accurate predictive models that estimate house prices in Nigeria, providing valuable insights to Wazobia Real Estate Limited for informed decision-making and improved market competitiveness.

### Data Overview

- Number of Entries: 14,000
- Features: Bathroom, Bedroom, Parking Space, Property Location (loc), Property Type (title), Price
- Target Variable: Price

### Data Analysis Highlights

In our exploratory data analysis (EDA), we delved into various aspects of the dataset to understand its characteristics and relationships. Here are some key insights:

- The distribution of bathrooms, bedrooms, and parking spaces is explored, revealing trends and possible outliers.
- The distribution of property prices is analyzed, highlighting skewness and the presence of outliers.
- Missing values are identified in the "loc" and "title" columns, and recommendations are provided for handling them appropriately.
- Correlation analysis showcases the relationships between features and the target variable (price), guiding feature selection for modeling.
- Location-based and property type-based pricing trends are uncovered, offering insights for pricing strategies.

### Data Access

You can access the complete dataset and participate in the hackathon on the Zindi platform: [Wazobia Real Estate Hackathon Data](https://zindi.africa/competitions/free-ai-classes-in-every-city-hackathon-2023/data).

Explore, analyze, and build predictive models to contribute to Wazobia Real Estate's journey towards enhanced pricing strategies and market success!

---


## Data Preprocessing

### Data Cleaning

- Removed rows with missing values in 'loc' and 'title' columns.

- Filled missing values in 'bedroom', 'bathroom', and 'parking_space' columns with their respective medians.

### Features Engineering

- Added binary indicator variables 'is_lagos' and 'is_mansion' to capture location and property type effects.

- Created new features 'comfort_ind', 'size', and 'comfort_by_size' to capture property comfort and size insights.

- Categorized locations based on population density into 'population_density_level'.

- Encoded 'loc' column using TargetEncoder, enhancing model's understanding of location-price relationship.


## Machine Learning WorkLoad
### Model Building

- Utilized CatBoostRegressor with RMSE as the loss function for predicting house prices.

- Employed 5-fold cross-validation with shuffling using KFold to prevent overfitting.

### Model Evaluation

- Achieved a cross-validation RMSE score of 416,786, indicating prediction variance.

- Leaderboard (LB) score of 310,010 for performance on the competition's test dataset (1st Place Score).



#### Features Importance

- Top three important features: "loc_encoded," "title_rank," and "bedroom" (23.06%, 22.46%, 19.12%).

- Significant contributions from "is_mansion" (10.31%), "size" (9.63%), "is_lagos" (4.28%), and "comfort_by_size" (3.64%).

- "comfort_ind," "parking_space," and "bathroom" have relatively lower importance scores.

## 🔗 Links

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/frankfelixai/)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/frankfelixai)

