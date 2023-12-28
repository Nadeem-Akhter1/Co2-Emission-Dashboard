# Co2-Emission-Dashboard
# Problem Statement:
I aim to analyze and visualize environmental, social, and governance (ESG) scores for different countries based on their CO2 emissions, population, GDP, and other factors. Additionally, it includes a decision tree regression model to predict CO2 emissions per capita using various features related to economic and environmental factors. The code concludes with a dashboard created using Dash, a Python web framework, to interactively explore ESG-related data for selected countries.

# Approach to the Solution:

Data Loading and Preprocessing:

The code starts by importing necessary libraries, including pandas, NumPy, Plotly Express, Seaborn, Matplotlib, and scikit-learn. These libraries provide tools for data manipulation, visualization, and machine learning.
The code reads two CSV files ('owid-co2-data.csv' and 'owid-co2-codebook.csv') using pandas, dropping missing values, and assigning meaningful scores for environmental, social, and governance factors.
ESG Score Calculation and Visualization:

Environmental, social, and governance scores are calculated based on CO2 emissions, population, and GDP.
The ESG scores are visualized using an animated scatter plot with Plotly Express, showing the relationship between GDP, CO2 emissions, and population over time. This interactive plot allows users to explore how countries' ESG scores change annually.
Weighted ESG Score Calculation:

The code introduces a weighted approach to calculate an overall ESG score by assigning weights to different parameters such as CO2 emissions, population, GDP, etc.
The distribution of the calculated ESG scores is visualized using a histogram with Seaborn and Matplotlib, providing insights into the distribution of ESG performance across the dataset.
Decision Tree Regression Model:

The code utilizes scikit-learn to train a decision tree regression model to predict CO2 emissions per capita. Features for the model include GDP, CO2 emissions, cement CO2, coal CO2, oil CO2, gas CO2, energy per GDP, and temperature change from CO2.
The model is evaluated using mean squared error, and feature importances are displayed, indicating the contribution of each feature to the model's predictions.
Predictions vs. Actual Values Visualization:

The code visualizes the predictions vs. actual values using a scatter plot, helping to assess the performance of the decision tree regression model. A diagonal red dashed line represents a perfect prediction scenario.
ESG Dashboard with Dash:

The code creates an ESG dashboard using Dash, allowing users to interactively explore CO2 emissions and related metrics for selected countries.
The dashboard includes a dropdown for country selection and four charts: CO2 emissions over time, greenhouse gas emissions over time, CO2 emissions per capita, and CO2 emissions per GDP. These charts update dynamically based on user-selected countries.
Deployment:

The Dash web application is run locally in debug mode for testing and development. For production use, the application could be deployed on a web server or cloud platform.

# Dataset
I have taken this dataset from: https://github.com/owid/co2-data
