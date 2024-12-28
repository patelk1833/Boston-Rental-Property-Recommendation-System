# Boston Rental Property Recommendation System
### By: Krish Patel
### Date: September 23rd, 2024

## Project Overview
This project leverages ***data analysis*** and ***machine learning*** to develop a ***recommendation system*** for rental properties in Boston, specifically designed for students at Wentworth Institute of Technology (WIT). The system aims to address the challenges of Boston’s ***competitive rental market*** by providing actionable insights into ***affordable***, ***accessible***, and ***user-preferred*** housing options.

By integrating ***rental price data***, ***property characteristics***, and ***travel time metrics***, this project tackles critical issues such as high demand and limited affordable options near universities. The objective is to identify properties that ***balance cost and convenience***, simplify the ***decision-making process***, and utilize ***data-driven approaches*** to deliver personalized recommendations, ultimately enhancing housing choices for students.

## Project Objectives
1. **Data Collection and Preparation:**
   - Gather rental property data using the HomeHarvest Library.
   - Retrieve travel times from properties to WIT via the Google Distance Matrix API.

2. **Data Analysis:**
   - Analyze rental price trends by location and property features.
   - Evaluate the impact of travel times on rental prices.

3. **Feature Engineering:**
   - Develop metrics such as price per minute of travel and neighborhood scores.
   - Create features to optimize the recommendation model.

4. **Model Development:**
   - Implement a Random Forest Regressor for rental price prediction.
   - Build a recommendation system tailored to user-defined constraints.

5. **Insights and Recommendations:**
   - Highlight properties with the best trade-offs between affordability and accessibility.
   - Provide actionable recommendations for students based on preferences.
  
## Methodology
1. **_Data Preparation:_** Real-time rental data from Boston was **_scraped_** using advanced tools to ensure accuracy. Walking, transit, and driving times were **_calculated_** with the help of the **_Google Distance Matrix API_** to provide comprehensive travel metrics. The data underwent **_cleaning and pre-processing_** to prepare it for analysis and modeling, ensuring high-quality and reliable input for the project.

2. **_Feature Engineering:_** Key metrics such as **_price_per_sqft_**, **_bed_bath_ratio_**, and **_neighborhood_travel_score_** were **_developed_** to better characterize the properties and their accessibility. These features played a pivotal role in analyzing **_travel costs_** and **_property characteristics_** to enhance the recommendation system's accuracy.

3. **_Exploratory Data Analysis (EDA):_**  Trends in **_rental prices_**, **_property features_**, and **_travel times_** were **_visualized_** using interactive plots, providing a clear understanding of the market. **_Spatial distribution patterns_** of prices and affordability were **_analyzed_**, offering actionable insights into the housing landscape in Boston.

4. **_Machine Learning:_** A **_Random Forest Regressor_** was **_trained and evaluated_** to predict rental prices effectively. The model achieved an impressive **_Root Mean Squared Error (RMSE)_** of 555.94, demonstrating its reliability and accuracy in price prediction.

5. **_Recommendation System:_** Properties were **_filtered_** based on user-defined constraints such as price and accessibility preferences. The system **_ranked_** the properties by balancing **_affordability_** and **_accessibility_**, offering students the best possible housing options tailored to their needs.

## Key Findings
- **Impact of Travel Times:**
  - Shorter travel times to WIT were associated with higher rental prices, reflecting a convenience premium.
  - Transit and walking times were significant factors influencing property desirability.
- **Property Features:**
  - Bedrooms and bathrooms had a strong correlation with rental prices.
  - Features like `price_per_sqft` and `bed_bath_ratio` provided valuable insights into property value.
- **Neighborhood Insights:**
  - Certain neighborhoods offered better trade-offs between affordability and convenience.
  - Properties within a 20-minute transit radius of WIT were most desirable.
 
 ## Conclusion
The Boston Rental Property Recommendation System successfully utilized data analysis and machine learning to address the challenges faced by students in finding affordable and accessible housing. By analyzing rental prices, property features, and travel times, the system provided actionable recommendations tailored to user-defined constraints. This project demonstrated a robust integration of data-driven insights and predictive modeling to enhance decision-making and deliver meaningful solutions to improve housing options for students.

## Future Scope
- Expand the system to include more cities and universities.
- Integrate additional property features such as energy efficiency and proximity to amenities.
- Enhance the model with advanced algorithms like Gradient Boosting and Neural Networks.

## Tools and Technologies
- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **APIs**: HomeHarvest Library, Google Distance Matrix API
- **Machine Learning Model**: Random Forest Regressor

## Repository Files

### Datasets

#### Raw Data
- [HomeHarvest_Boston_Rentals.xlsx](https://github.com/patelk1833/Boston-Rental-Property-Recommendation-System/tree/main/datasets/raw): Contains the raw data scraped from the HomeHarvest Library for rental properties in Boston.

#### Cleaned Data
- [HomeHarvest_Boston_Rentals_Cleaned.xlsx](https://github.com/patelk1833/Boston-Rental-Property-Recommendation-System/tree/main/datasets/cleaned): Data after initial cleaning for missing values and duplicates.
- [HomeHarvest_Boston_Rentals_Cleaned_with_Room_Stats.xlsx](https://github.com/patelk1833/Boston-Rental-Property-Recommendation-System/tree/main/datasets/cleaned): Cleaned data enriched with room-related metrics.
- [HomeHarvest_Boston_Rentals_with_Travel_Times.xlsx](https://github.com/patelk1833/Boston-Rental-Property-Recommendation-System/tree/main/datasets/cleaned): Cleaned data merged with travel time metrics calculated using the Google Distance Matrix API.

#### Final Data
- [HomeHarvest_Boston_Rentals_Final.xlsx](https://github.com/patelk1833/Boston-Rental-Property-Recommendation-System/tree/main/datasets/final): Final dataset used for modeling and analysis.
- [recommended_properties.xlsx](https://github.com/patelk1833/Boston-Rental-Property-Recommendation-System/tree/main/datasets/final): Recommended properties generated from the machine learning model.

### Graphs
- [Travel Time Impact Analysis](https://github.com/patelk1833/Boston-Rental-Property-Recommendation-System/tree/main/graphs): Contains visualizations analyzing the relationship between travel times (walking, transit, and driving) and rental prices.
- [Property Characteristics Analysis](https://github.com/patelk1833/Boston-Rental-Property-Recommendation-System/tree/main/graphs): Includes graphs showing insights from property-specific features such as bedrooms, bathrooms, and price per square foot.
- [Location-Based Analysis](https://github.com/patelk1833/Boston-Rental-Property-Recommendation-System/tree/main/graphs): Contains heatmaps and geospatial plots related to neighborhood scores and accessibility.

### Documents
- [Final Paper: Final_Paper_Krish_Patel.pdf](https://github.com/patelk1833/Boston-Rental-Property-Recommendation-System/blob/main/documents/Final%20Paper_Krish%20Patel.pdf): PDF version of the final project report.

### Notebook
- [Boston_Rental_Property_Recommendation_Project.ipynb](https://github.com/patelk1833/Boston-Rental-Property-Recommendation-System/blob/main/notebook/Boston_Rental_Property_Recommendation_Project.ipynb): Jupyter notebook containing all the code, analysis, and model development for the project.







