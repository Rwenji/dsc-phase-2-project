# Falcon Real Estate Analysis

## Introduction

This project focuses on Falcon Real Estate agencies, a well-established real estate firm located in King County, USA, that is seeking assistance in identifying the primary factors that affect property values within the region. The agency aims to leverage this knowledge to inform their pricing strategies for residential properties.

### Research Questions

- What are the key factors that determine the prices of houses in the real estate market?
- Which specific features have a positive impact on the value of a house, and which ones have a negative impact?
- How can the predictive model help distinguish between overpriced and underpriced properties in the market?
- In what ways can analytical insights and a refined pricing strategy be employed to increase the annual revenue of the real estate agency and achieve a more profitable operation?

## Objectives

#### Main Objective
- To create an optimal predictive model that will enable the agency to accurately establish competitive property prices.

#### Specific Objectives

- To understand which factors determine the prices of houses.
- To explore which features will decrease and increase the value of the house.
- To distinguish between overpriced and underpriced properties by juxtaposing the predicted prices with the actual selling prices.
- To bolster the annual revenue of the agency by employing the analytical insights and refined pricing strategy, thus achieving a more profitable real estate operation.


## Exploratory Data Analysis

This project utilized univariate analysis to examine the distribution and characteristics of individual variables, while bivariate analysis focused on exploring relationships between variables.Different plots were utilized to visualize the correlation between numerical and categorical variables with the house prices. Multivariate analysis incorporated a heatmap to display the correlation between all columns in the dataset.


## Data Analysis and Modeling
Two models were developed during the project.A simple linear regression, established the initial understanding of the relationship between the square footage of living space and house prices. From the simple linear model, it was observed the model wasn't the best for this analysis.The model's R2 value was extreemly low, indicating that there are other numerous factors in housing that affect the house prices.Therefore, we had to do the multiple linear regression. OneHot Encoding that was initially introduced to convert the categorical variables to binary representation was suitable for machine learning algorithms. The second model certainly improved from the baseline model. The R2 was at 55.8%; The F-statistic of 3003.0 with a probability (p-value) of 0.00 suggests that the overall model is statistically significant, meaning that at least one of the independent variables has a significant effect on the dependent variable.
Among the independent variables, 'const', 'sqft_living', 'bathrooms', 'bedrooms', 'floors', 'condition_Avarage ', and 'condition_Fair' exhibit statistical significance, with p-values below our significance level (alpha of 0.05). This indicates that these variables have a substantial impact on 'price'. In contrast, 'condition_Good', 'condition_Poor'and condition_Very_Good' have p-values exceeding our alpha of 0.05, at 0.074 ,0.046 and 0.255, respectively, implying that they are not 'statistically significant in predicting 'price'.

## Conclusion

According to the Ordinary Least Squares (OLS) regression results, the multiple linear regression model created to determine the primary factors influencing house prices in the northwestern county possesses an adjusted R-squared value of 0.558, indicating that it can account for approximately 55.8% of the variation in house prices using the selected features. The model is statistically significant, as evidenced by the F-statistic of 3,003 and a corresponding p-value of 0.00.

Several features exhibit significant impacts on house prices in the region. Notable factors include the square footage of the living area (sqft_living),floor,age,the house condition, the number of bedrooms and bathrooms,

The developed model can serve as a valuable tool for determining optimal pricing strategies for the real estate agency. It offers coefficients for each feature, enabling the agency to estimate property prices more accurately by considering these coefficients and the property's specific attributes. Additionally, by comparing predicted prices with actual prices, the agency can pinpoint overpriced or underpriced homes and make necessary adjustments to maximize sales potential.

The analytical insights and pricing strategies derived from this project can make a substantial contribution to enhancing the agency's annual revenue. Leveraging the model's findings and implementing the recommended pricing strategies will empower the agency to improve decision-making, attract potential buyers, and increase the volume of homes sold.

## Recommendation

majority of buyers are looking for houses with fewer bedrooms, it may be beneficial to focus on
properties with a lower bedroom count

An increase in the number of bathrooms tends to have a positive impact on the house price. If feasible,
consider adding or upgrading bathrooms in properties to attract buyers who value this feature

Houses with multiple floors tend to have higher prices. If feasible, explore opportunities to add or
emphasize multiple floors in properties to increase their perceived value

Increasing the size of the living space generally increases the house price, while larger lot sizes may
have a slight negative impact. It’s good to consider the preferences of the target market.

The condition and the age of the property does not have a significant impact on the price