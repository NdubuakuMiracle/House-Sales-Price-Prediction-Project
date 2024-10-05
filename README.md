# House Sales Price Prediction Project  

## Project Overview  

RealAgents is a real estate company specializing in the sale of houses within a metropolitan area. The company deals with various types of houses that exhibit differing sales velocities, sometimes necessitating price reductions to secure buyers. To remain competitive in the market, RealAgents aims to optimize the listing prices of houses by predicting their sale prices based on specific characteristics. By accurately predicting these prices, the company seeks to reduce the time each house spends on the market.  

## Dataset Description  

The dataset utilized for this project contains records of houses sold in the area, with the following criteria for each column:  

| Column Name       | Criteria                                                                                          |  
|-------------------|---------------------------------------------------------------------------------------------------|  
| **house_id**      | **Nominal.** Unique identifier for houses. Missing values are not permitted.                     |  
| **city**          | **Nominal.** The city where the house is located. Possible values: 'Silvertown', 'Riverford', 'Teasdale', 'Poppleton'. Missing values are replaced with "Unknown". |  
| **sale_price**    | **Discrete.** The sale price of the house, recorded in whole dollars. This value must be a positive number (≥ 0). Missing entries are removed from the dataset. |  
| **sale_date**     | **Discrete.** The date of the last sale of the house. Missing values are replaced with '2023-01-01'. |  
| **months_listed** | **Continuous.** The number of months the house was listed before the last sale, rounded to one decimal place. Missing values are replaced with the mean number of months listed, also rounded to one decimal place. |  
| **bedrooms**      | **Discrete.** The number of bedrooms in the house, with permissible values being positive integers (≥ 0). Missing values are replaced with the mean number of bedrooms, rounded to the nearest integer. |  
| **house_type**    | **Ordinal.** The type of house: "Terraced" (two shared walls), "Semi-detached" (one shared wall), or "Detached" (no shared walls). Missing values are replaced with the most common house type. |  
| **area**          | **Continuous.** The area of the house measured in square meters, rounded to one decimal place. Missing values are replaced with the mean area, rounded to one decimal place. |  

## Methodology  

1. **Data Cleaning**: Initially, the dataset was cleaned to handle any missing values according to the defined criteria. Specific strategies, such as replacing missing values with the mean or most common values, were employed to maintain dataset integrity.  

2. **Feature Selection**: Relevant features that could influence the sale price were identified, including city, months listed, bedrooms, house type, and area.  

3. **Price Prediction Model**: A predictive model was developed to estimate house sale prices based on the identified features. Various algorithms—such as linear regression, decision trees, and random forests—were tested to determine the most effective modeling approach.  

4. **Model Evaluation**: The model was evaluated using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²) to assess prediction accuracy and validate the model's effectiveness.  

5. **Implementation**: Once an optimal model was identified, it was applied to predict sale prices of houses in the current listings, enabling RealAgents to adjust their pricing strategies proactively.  

## Conclusion  

By predicting the sale price of houses based on their characteristics, RealAgents aims to optimize its pricing strategies and ultimately reduce the time taken to sell properties. The project successfully established a structured approach to price prediction, which can enhance the company’s competitiveness in the real estate market.
