# Fridge-price-determinant-analysis
Statistical analysis of refrigerator pricing factors using R (Linear Regression, ANOVA) combined with a normalized database design (ERD).

🧊 Fridge Price Predictor: Data Normalization & Price Determinant Analysis
This project performs Database Normalization (ERD Design) based on raw refrigerator specification data and utilizes R to statistically analyze and predict key variables influencing market prices.

🛠 Tech Stack
Language: R

Library: tidyverse (dplyr, ggplot2), broom

Database Design: Entity Relationship Diagram (ERD)

💾 Database Design (ERD)
To ensure data integrity and analytical efficiency, the unstructured CSV dataset was normalized into three logical entities: BRAND, PRODUCT, and PRICE.

<img width="1312" height="676" alt="사진" src="https://github.com/user-attachments/assets/39a81cca-f62f-4e25-8dec-05eab1448b2e" />

[Key Design Strategies]
Normalization: Separated brand details and product specifications to eliminate data redundancy and enhance maintainability.

Scalability: Designed PRICE as an independent table to easily accommodate future data such as price history across different retailers or time-series price fluctuations.

Logical Dependency: Established a structure where Price is primarily dependent on Brand and Country of Manufacture, ensuring that market-specific pricing strategies and brand positioning are accurately reflected in the data model.

📊 Data Analysis & Insights
Key findings from the Exploratory Data Analysis (EDA) and Regression Modeling using R:

1. Statistical Significance Testing
Conducted ANOVA to verify whether 'Brand' and 'Country of Manufacture' lead to statistically significant differences in price.

2. Price Determinant Modeling (Regression Analysis)

Key Variables: Capacity, Energy Efficiency Rating, Country of Manufacture, etc.

Findings: Linear regression analysis revealed that typical hardware specifications have no statistically significant impact on price variations. The low coefficients and p-values for these variables indicate that physical features are no longer the primary drivers of cost in the current market.

Interpretation: This "lack of significance" suggests that technical specs have become a baseline (standardized) rather than a premium differentiator.

[Overall Conclusion & Strategic Insights]

Based on the findings, I propose the following strategic directions for home appliance manufacturers:

Shift from R&D to Brand Positioning: As hardware specifications (capacity, materials) undergo technological commoditization, incremental technical upgrades no longer justify high price premiums. Companies should reallocate resources from pure technical R&D to Brand Storytelling and Lifestyle Positioning.
