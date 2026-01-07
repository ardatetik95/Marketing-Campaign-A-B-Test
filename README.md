# Marketing-Campaign-A-B-Test
This project evaluates the effectiveness of three marketing promotions using A/B testing methods.

Dataset from: https://www.kaggle.com/datasets/chebotinaa/fast-food-marketing-campaign-ab-test

About the Dataset

A fast-food chain plans to add a new item to its menu. However, they are still undecided between three possible marketing campaigns for promoting the new product. In order to determine which promotion has the greatest effect on sales, the new item is introduced at locations in several randomly selected markets. A different promotion is used at each location, and the weekly sales of the new item are recorded for the first four weeks.

Columns:

MarketID: unique identifier for market 

MarketSize: size of market area by sales 

LocationID: unique identifier for store location 

AgeOfStore: age of store in years 

Promotion: one of three promotions that were tested 

week: one of four weeks when the promotions were run 

SalesInThousands: sales amount for a specific LocationID, Promotion, and week



**About the Project**

This project evaluates the effectiveness of three marketing promotions using a statistically robust A/B testing framework.
Due to unequal variances and non-normal sales distributions, Welch’s ANOVA and Games–Howell post-hoc testing were applied.

**Goal:**

Identify whether different promotions lead to statistically and practically significant differences in sales

**Business Question **

Do different promotions generate significantly different sales outcomes, and which promotion performs best? 

**Experimental Design**

**Independent Variable:** Promotion type (3 levels)  
**Dependent Variable:** Sales (in thousands)  
**Observations:** Independent sales outcomes 

**Hypotheses**

**H0:** Mean sales are equal in all promotion types
**H1:** At least one of the mean sales is different.

**Tests Used and Methodology**

- Shapiro-Wilk for Normality Assumption -> Large sample sensitivity
  
- Levene’s Test for Variance Homogeneity Assumption -> Homogeneity violated
  
- Welch’s ANOVA for Statistical Testing (Good for unequal variances)
  
- Games-Howell for Post-Hoc Testing (Also good for unequal variances)

**Results:**

Promotion 2 performed worse than 1 and 3, it should be redesigned and reconsidered.

Promotion 1 and 3 have close values, they can be used in our business.

**Required Libraries**

pandas

scipy

pingouin


**Skills Demonstrated:**

- A/B testing and experimental design
- 
- Assumption diagnostics
- 
- Welch ANOVA & Games–Howell testing
- 
- Business-driven statistical reasoning
- 
- Clean and reproducible analysis 

Coding parts can be seen in the “Marketing AB Test.ipynb” file.
