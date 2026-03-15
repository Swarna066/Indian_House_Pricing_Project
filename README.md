# Indian House Price Prediction & Market Analysis

## 📌 Project Overview
This project leverages machine learning and statistical modeling to predict residential property prices across India using a dataset of approximately **250,000 observations**. We explored several regression techniques—from traditional Linear Models to advanced Random Forests—to identify the key drivers of real estate value.

## 📊 About the Data
The dataset contains listings of properties across various Indian states. Key features analyzed include:
* **Price_in_Lakhs**: The target variable (1 Lakh = 100,000 INR).
* **BHK**: Number of Bedrooms, Hall, and Kitchen (indicates property size/type).
* **Median_Price_Locality**: An engineered feature capturing the baseline property value of the surrounding neighborhood.
* **Size_in_SqFt**: Total square footage of the property.
* **Property_Type**: Categorical indicator (e.g., Villa, Apartment).

## 🚀 Key Technical Features
* **Multi-Model Evaluation**: Conducted a comparative analysis of **Linear Models (LM)**, **Generalized Linear Models (GLM)**, **Decision Trees**, and **Random Forests**.
* **Variable Importance Analysis**: Discovered that **Locality** is the dominant price driver in the Indian market, holding a **99.94% importance score**, far outweighing physical size.
* **Statistical Rigor**: Performed extensive hypothesis testing, including **F-tests (var.test)**, to validate variance assumptions (Homoscedasticity) across different property types like Villas and Apartments.
* **Interactive Dashboard**: Built and deployed a live **R Shiny App** allowing users to filter and explore market trends dynamically.

## 📈 Model Performance Results
| Model | Mean Absolute Error (Lakhs) | Root Mean Square Error (Lakhs) |
| :--- | :--- | :--- |
| **Linear Model (Winner)** | **79.15** | **99.05** |
| **Decision Tree** | 115.27 | 136.71 |
| **Random Forest** | 118.21 | 137.97 |
| **GLM (Gamma)** | 128.95 | 422.26 |

*Note: The Linear Model was selected as the final champion due to its high stability across the price spectrum and resilience against luxury outliers compared to the GLM.*

## 🛠️ Tech Stack
* **Language**: R
* **Libraries**: `tidyverse`, `randomForest`, `rpart`, `shiny`, `ggplot2`
* **Reporting**: Quarto / R Markdown

## 🔗 Project Links
* **Live Dashboard**: (https://atreyaghoshal.shinyapps.io/indian_housing_shiny/)

* **Project Documentation**: https://swarna066.github.io/Indian_House_Pricing_Project/Project.html
