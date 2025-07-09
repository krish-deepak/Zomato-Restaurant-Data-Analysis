# Zomato-Restaurant-Data-Analysis
Zomato Restaurant Data Analysis and insights 

  * "Conducted an in-depth EDA on the Zomato dataset to identify key drivers of restaurant performance."
  * "Revealed a strong correlation between price range, customer votes, and aggregate ratings, providing a clear success metric for restaurant partners."
  * "Translated raw data into actionable business insights, such as identifying competitive cuisine markets and recommending premium features for high-end restaurants and pricing details."
-----

# Zomato Restaurant Data Analysis

### Project Analysis & Methodology

This project performs a comprehensive exploratory data analysis (EDA) on the Zomato restaurant dataset and follows a structured data analysis workflow, beginning with data wrangling and feature engineering, and culminating in actionable business intelligence. The primary goal is to uncover key insights into the factors that influence a restaurant's success, such as location, cuisine, cost, and customer ratings. The analysis aims to provide actionable recommendations for both restaurant owners and Zomato's business strategy.

### Dataset

The dataset contains information for thousands of restaurants, encompassing various attributes like location, cuisine type, average cost, user ratings, and service options (e.g., table booking, online delivery).

### Key Libraries Used

  * **Data Manipulation & Analysis:** `pandas`,`numpy`
  * **Data Visualization:** `matplotlib`, `seaborn`

-----

## Analysis & Key Findings 📈

The analysis systematically explores the dataset, starting from data cleaning and moving toward uncovering deep insights through visualization.

### 1\. Data Cleaning & Preparation

  * The initial dataset was loaded and inspected for inconsistencies.
  * Null values, particularly in the `Cuisines` column, were handled appropriately.
  * Features were transformed to ensure data integrity for accurate analysis.

### 2\. Geographical Distribution Analysis

  * **Insight:** The majority of restaurants in the dataset are concentrated in **India**, with **New Delhi** having the highest density of listings.
  * **Business Implication:** This highlights India as a critical market for Zomato. Marketing and operational strategies should be tailored for high-density cities like New Delhi, which show a highly competitive restaurant landscape.

![image](https://github.com/user-attachments/assets/22fb9289-64a2-4644-be95-48c486fc872f)
![image](https://github.com/user-attachments/assets/3017070f-fff5-4743-baf9-18667befa084)


### 3\. Service & Cost Analysis

Synergistic Effects: Engineered a Service Combination feature to prove that offering bundled services (i.e., both Table Booking and Online Delivery) results in the highest average customer ratings.

  * **Insight 1: Online Delivery:** A significant number of restaurants offer online delivery. The analysis indicates that having an online delivery option is common across various price points but does not, on its own, guarantee a higher rating.
  * **Insight 2: Table Booking & Cost:** There is a strong positive correlation between offering **table booking** and having a **higher average cost**. Restaurants providing this service are typically in the premium price range.
  * **Business Implication:** Zomato could create premium subscription tiers for restaurants that highlight the "Table Booking" feature, targeting high-end establishments that focus on the dine-in experience.


![image](https://github.com/user-attachments/assets/bf3a8565-3a47-4416-a46c-e8c7673b276e)

![image](https://github.com/user-attachments/assets/41d59c55-cb42-4d27-8b4f-43f19ca8c6b9)


### 4\. Cuisine & Rating Analysis

  * **Insight 1: Popular Cuisines:** **North Indian** and **Chinese** cuisines are the most prevalent in the dataset, indicating their high demand and market saturation.
  * **Insight 2: Ratings Distribution:**The rating distribution is not a simple positive skew but is centered around a large base of 'Average' to 'Good' restaurants. The key business challenges and opportunities are twofold:
For Zomato: How to convert the large, silent 'Not rated' segment into active, rated listings.
For Restaurants: How to move from the crowded 'Average' category into 'Good' or 'Very Good' to gain a competitive edge.
  * **Business Implication:** For new restaurants, entering the North Indian or Chinese food market is highly competitive. A focus on niche cuisines with less competition could be a viable market entry strategy. Zomato can use this data to advise new restaurant partners.

 ![image](https://github.com/user-attachments/assets/0eebb27a-f135-406a-a488-74ff06c262a0)
 ![image](https://github.com/user-attachments/assets/0b4df1a1-e6b4-4bb9-9ae8-e2715c7155f2)



### 5\. Correlation & Feature Impact

  * **Key Finding:** The **'Aggregate rating'** shows a strong positive correlation with **'Votes'**, **'Price range'**, and **'Average Cost for two'**.
  * **Conclusion:** This is a critical insight. It proves that:
    1.  **Higher price points often correlate with higher ratings**, suggesting that customers who pay more have higher satisfaction, likely due to better quality and service.
    2.  **Higher engagement (more votes) is linked to higher ratings**, creating a positive feedback loop.
  * **Business Analyst Recommendation:** Zomato should encourage users to rate and review restaurants by gamifying the process. For restaurant owners, this proves that investing in a quality dining experience that justifies a higher price point is a key driver for achieving top ratings.
    Holistic Feature Relationships: Conducted a final correlation analysis, visualized with a heatmap, to synthesize all findings. This confirmed that Price Range, Votes, and the availability of Table Booking are the most powerful predictors of a high Aggregate rating.


### 6\. Feature Engineering & Global Cost Analysis

1. Currency Standardization
To create a uniform basis for comparison, the Average Cost for two column, which contained multiple local currencies, was systematically converted to a single standard currency (e.g., Indian Rupee - INR). This step was crucial for eliminating currency fluctuations as a variable and enabling direct cost comparisons.

2. Purchasing Power Parity (PPP) Conversion
To achieve a more accurate and economically sound comparison, a Purchasing Power Parity (PPP) feature was engineered. The standardized INR cost was converted to its PPP equivalent. This advanced transformation normalizes the cost data, allowing us to understand restaurant affordability relative to the local economy of each country.

Key Insights from Cost Analysis
With these robust new features, a cross-country analysis of dining costs yielded several key insights:

Global Cost Ranking: The analysis of average PPP costs revealed a clear hierarchy of dining affordability across the globe. Countries like the USA, UK, and Qatar emerged as having the highest average dining costs, while countries in Southeast Asia, including India and the Philippines, were identified as the most budget-friendly markets.

Dining Diversity (Min/Max Range): By examining the minimum and maximum cost for two in each country, we can gauge the diversity of the restaurant market.

High-Range Markets: Countries with a vast range between their minimum and maximum costs (e.g., USA) indicate a mature market with everything from cheap eats to exclusive fine dining.

Niche Markets: Countries with a narrower cost range suggest a less diverse market, potentially focused on a specific economic segment (e.g., budget or mid-range).
![image](https://github.com/user-attachments/assets/0933d318-618c-43d4-9d4d-89926331ebf0)


## Conclusion & Recommendations

This EDA provides a clear data-driven overview of the Zomato ecosystem. The most successful restaurants are those that manage to align their price point with a high-quality experience, leading to better ratings and higher customer engagement.




