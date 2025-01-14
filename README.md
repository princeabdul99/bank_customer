# Project Background
**Bank Customer Churn**

Account information for 10,000 customers at a European bank, including details on their credit score, balance, products, and whether they have churned.

This project utilizes data visualization techniques to uncover insights into customer churn and behavior within a bank.

Insights and recommendations are provided on the following key areas:
- **Churn Attributes and Predictability:** dentifying attributes that are more prevalent among churners compared to non-churners and assessing the predictive power of the available variables.
- **Customer Demographics:** Analyzing the overall demographic profile of the bank’s customers to understand key characteristics. 
- **Regional Behavior Differences:** Exploring account behavior differences among German, French, and Spanish customers.
- **Customer Segmentation:** Identifying distinct customer segments based on demographic and behavioral patterns.

An interractive PowerBI dashboard can be accessed [here](https://app.powerbi.com/view?r=eyJrIjoiZGIxNDQ3ZjItZmZjMS00YzQzLWEzZTYtYTkwZWU1YmY0ZWFhIiwidCI6IjJkZTU1ZjVjLWQwMDMtNGQyYS04MjZiLWVhZDJhOWYyYjljZCJ9)

# Data Structure & Initial Checks
The CSV data file consist of a table with total row count of 10,000 records.
![image_alt](https://github.com/princeabdul99/bank_customer/blob/d1725e6eebb55f4f382af8ac636ef6d9a4a72e00/Org%20Chart%20Flowchart%20Whiteboard%20in%20Violet%20Purple%20Adjacent%20Color%20Blocks%20Style%20(3).png)  

Prior to begining the analysis, a variety of checks where conducted for quality control and familiarization with datasets. The raw data file can be found [here](https://github.com/princeabdul99/bank_customer/blob/90f5c5fd915a49188df3e6d663bc1761371fc123/Bank%2BCustomer%2BChurn.zip)

# Executive Summary

### Overview Findings

The analysis highlights key regional differences in customer behavior and their correlation with churn. German customers have the highest average account balances ($119.73k) and a balanced gender ratio, making them ideal for premium services and wealth management strategies. Conversely, Spain faces challenges with the highest proportion of customers with zero account balances (1,199) and a significant low-income demographic (10.7%), requiring targeted financial inclusion initiatives. France leads in inactive customers (48.33%), signaling an opportunity for re-engagement campaigns. Across regions, tenure is stable, with most customers having 6+ years, offering a solid base for loyalty and retention programs.

Churn analysis further reveals that churners have a higher proportion of inactive customers (63.92%) and slightly lower credit scores (646 vs. 653). Churners are more evenly distributed geographically, with higher concentrations in Germany (39.96%) and Spain (20.27%), compared to non-churners who are predominantly from France. Gender dynamics also play a role, as churners include more females (55.92%) than non-churners (42.75%).


Below is the overview page from the Power BI dashboard and more examples are included throughout the report. The entire interractive dashboard can be accessed [here](https://app.powerbi.com/view?r=eyJrIjoiZGIxNDQ3ZjItZmZjMS00YzQzLWEzZTYtYTkwZWU1YmY0ZWFhIiwidCI6IjJkZTU1ZjVjLWQwMDMtNGQyYS04MjZiLWVhZDJhOWYyYjljZCJ9)




#### Churn Attributes and Predictability:

|                      | Chuner | Non-Churner |
|----------------------|--------|-------------|
| Active Customers     | 735    | 4416        |
| Inactive Customers   | 1,302  | 3547        |
| Median Credit Score  | 646    | 653         |
| **Country Distribution**                    |
| Spain                | 20.27% | 25.92%      |
| France               | 39.76% | 52.79%      |
| Germany              | 39.96% | 42.75%      |
| **Gender Distribution**                     |
| Male                 | 44.08% | 57.25%      |
| Female               | 55.92% | 42.75%      |

![image_alt](https://github.com/princeabdul99/bank_customer/blob/a68989dc02f76edd30e211e815592d8d198dd7f1/churn.jpg)  

##### Common Attributes Among Churners Compared to Non-Churners
- **Account Activity:**  
  Churners have a higher proportion of inactive customers (63.92%) compared to non-churmers (44.54%)
- **Account Balance:**  
  Churners tend to have a higher median account balance ($109.35k) than non-churners ($290.07k).
- **Credit Score:**  
  Churners generally have slightly lower median credit scores (646) compare to non-churners (653).
- **Country Distribution:**  
  Churners are more evenly distributed across countries, with higher proportions in Germany (39.96%) and Spain (20.27%) compared to non-churners, who are predominantly from France (52.79%).
- **Gender Distribution:**  
  Churner include a higher percentage of famales (55.92%) compared to non-churners (42.75%)       


#### Customer Demographics:
- **Country Distribution:**
  The majority of customers are from France (50.14%), followed by Germany (25.09%) and Spain (24.77%).
- **Gender Proportion:**
  Males make up a slightly larger portion of the customer base (54.57%) compared to females (45.43%).
- **Age Distribution:**  
      - The largest age group is 30-39 years, representing 44.46% of the customers.  
      - The 40-49 age group follows, comprising 26.18% of the customers.  
      - Younger customers (19 & below) make up only 0.49%, while older customers (60 & above) represent 5.26%.


#### Regional Behavior Differences:
- **Account Balance:**
    - German customers have significantly higher average account balances ($119.73k) compared to customers in France ($62.09k) and Spain ($61.82k).
    - Spain has the highest proportion of customers with zero account balances (1,199), while Germany has none.

- **Inactive Customers:**
    - France has the highest number of inactive customers (2,423 or 48.33%), followed by Spain (1,165 or 47.04%) and Germany (1,261 or 50.25%).
 
- **Gender Distribution:**
    - Spain has the highest proportion of male customers (56.04%), while Germany has a more balanced gender ratio (male: 52.45%, female: 47.55%).
 
- **Tenure:**
    - Across all countries, the distribution of tenure is relatively similar, with the largest group having 6 years or more (France: 45.21%, Germany: 44.36%, Spain: 44.97%).

- **Credit Score Ratings:**
    - Spain has the highest proportion of customers with fair credit scores (34.03%), while Germany has a slightly higher proportion of customers with excellent credit scores (7.01%) compared to France (6.44%) and Spain (6.03%).

- **Salary Ratings:**
    - High-income customers dominate in all countries but are most prominent in Germany (50.9%), followed by Spain (49.98%) and France (49.76%).
    - Spain has the highest proportion of low-income customers (10.7%).

- **Product Engagement:**
    - Customers with 1 product are most common in all regions, but Spain has the highest proportion (1,221 or 49.28%).
    - Germany has a slightly higher proportion of customers with 3 or 4 products (96 and 24, respectively) compared to France and Spain.

#### Customer Segmentation:
- **High-Value Engaged Customers:**
    - **Demographics:** Predominantly German, male, aged 30-49.
    - **Behavioral Patterns:**
      - High account balances (average: $119.73k).
      - High income (50.9% are high-income earners).
      - More likely to have multiple products (2+ products: 44%).
      - Low rate of zero account balances (0%).


- **Moderate-Value Loyal Customers:**
    - **Demographics:** French, evenly distributed across genders, aged 30-49.
    - **Behavioral Patterns:**
      - Average account balance ($62.09k).
      - High income (49.76% are high-income earners).
      - Predominantly engaged with 1-2 products (97.28%).
      - Balanced tenure distribution, with the majority having 6+ years (45.21%).
      - Higher inactivity rate (48.33%).


- **Low-Value Passive Customers:**
    - **Demographics:** Spanish, male-dominant, aged 20-39.
    - **Behavioral Patterns:**
      - Lower account balances ($61.82k).
      - High prevalence of zero account balances (1,199 or 48.41%).
      - Predominantly engaged with 1 product (49.28%).
      - A significant portion falls under low or mid-income categories (24.83%).


- **At-Risk Inactive Customers:**
    - **Demographics:** Spread across all regions, predominantly female, aged 40-59.
    - **Behavioral Patterns:**
      - High inactivity rates, particularly in France (48.33%) and Spain (47.04%).
      - Lower product engagement (1 product).
      - Higher proportion of fair and poor credit scores (France: 56.66%, Spain: 57.12%).


- **High-Potential Young Customers:**
    - **Demographics:** Aged 19-29, primarily male, balanced across all regions.
    - **Behavioral Patterns:**
      - Moderate account balances.
      - Lower tenure (1 year or less: ~14%).
      - Minimal product engagement (1 product).
      - Opportunity to increase engagement with targeted offers.


### Recommendations:
Based on the unconvered insights, the following recommendations have been provided;
- Focus on re-engagement campaigns for inactive customers. Offer personalized incentives or reminders to encourage account activity and interaction with services.
- Provide credit score improvement resources or tailored financial products for customers with lower credit scores to improve their financial stability and loyalty.
- Develop region-specific retention strategies. For instance, analyze customer needs and preferences in Germany and Spain to design targeted offers and services.
-  Investigate gender-specific needs and preferences. For example, assess the accessibility and inclusivity of services for female customers and adapt marketing efforts to resonate more with this demographic.

### Conclusion:
To address these findings, the organization should adopt region-specific retention strategies, such as re-engagement campaigns for inactive customers in France and Germany, financial education initiatives in Spain, and premium service promotions in Germany. By aligning products and engagement efforts with regional and churn-specific insights, the company can strengthen customer relationships, reduce churn, and drive sustained growth.
  







  








