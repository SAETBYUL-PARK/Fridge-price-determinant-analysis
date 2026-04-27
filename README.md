# Fridge-price-determinant-analysis
Statistical analysis of refrigerator pricing factors using R (Linear Regression, ANOVA) combined with a normalized database design (ERD).

🧊 Fridge Price Predictor: Data Normalization & Price Determinant Analysis
This project performs Database Normalization (ERD Design) based on raw refrigerator specification data and utilizes R to statistically analyze and predict key variables influencing market prices.

🛠 Tech Stack
Language: R

Library: tidyverse (dplyr, ggplot2), broom

Database Design: Entity Relationship Diagram (ERD)

💾 Database Design (ERD)
To ensure data integrity and analytical efficiency, the unstructured CSV dataset was normalized into two logical entities: BRAND, PRODUCT.

<img width="892" height="757" alt="캡처1" src="https://github.com/user-attachments/assets/3855889e-235c-43c2-937c-36a1288ff6b2" />


[Key Design Strategies]
Normalization: Separated brand details and product specifications to eliminate data redundancy and enhance maintainability.

Logical Dependency: Established a structure where Price is primarily dependent on Brand and Country of Manufacture, ensuring that market-specific pricing strategies and brand positioning are accurately reflected in the data model.

📊 Data Analysis & Insights
Key findings from the Exploratory Data Analysis (EDA) and Regression Modeling using R:

<details>
<summary><b>Click to expand the 8 research hypotheses</b></summary>
  1. **Manufacturing Origin & Warranty Premium**
   * Hypothesis: The impact of warranty periods on price premiums will show an exponential increase specifically for products manufactured in high-cost regions.
  
1. Statistical Significance Testing
Conducted ANOVA to verify whether 'Brand' and 'Country of Manufacture' lead to statistically significant differences in price.

2. Price Determinant Modeling (Regression Analysis)

Key Variables: Capacity, Energy Efficiency Rating, Country of Manufacture, etc.

Findings: Linear regression analysis revealed that typical hardware specifications have no statistically significant impact on price variations. The low coefficients and p-values for these variables indicate that physical features are no longer the primary drivers of cost in the current market.

<img width="596" height="528" alt="사진" src="https://github.com/user-attachments/assets/0a22ef77-c759-48a7-ae48-213964ab2cc1" />

Interpretation: This "lack of significance" suggests that technical specs have become a baseline (standardized) rather than a premium differentiator.

[Overall Conclusion & Strategic Insights]

Based on the findings, I propose the following strategic directions for home appliance manufacturers:

Shift from R&D to Brand Positioning: As hardware specifications (capacity, materials) undergo technological commoditization, incremental technical upgrades no longer justify high price premiums. Companies should reallocate resources from pure technical R&D to Brand Storytelling and Lifestyle Positioning.

## Data source
[fridge_price_predictor_datasets_real_brands.csv on Kaggle](https://www.kaggle.com/datasets/souradippal/fridge-price-prediction-dataset)

