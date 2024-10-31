# Housing Price Prediction Analysis

## Executive Summary
This analysis utilizes an OLS model to predict housing prices in Bangkok and its vicinity, focusing on three property types: Condos, Detached Houses, and Townhouses. The objective is to evaluate which investment offers better returns: real estate or stocks. Our findings reveal that while Bangkok properties command higher prices, location, size, and accessibility significantly influence property values. Notably, Nonthaburi and Samut Prakan have lower prices but are impacted by developments like the Eastern Economic Corridor (EEC).

## Key Insights
- **Location Matters:** Properties in Nonthaburi and Samut Prakan are generally cheaper compared to Bangkok, yet the EEC may boost future values.
- **Size and Functionality:** Property characteristics must align with market demand. Townhouses tend to be less valuable than Condos, and Detached Houses also show decreased values.
- **Accessibility:** Proximity to public transport stations correlates with higher property prices.

## OLS Regression Model

### Model Summary
- **Dependent Variable:** price_scaled
- **R-squared:** 0.517
- **Observations:** 14,103
- **Statistical Significance:** All factors analyzed show significant effects on property pricing.


# OLS Regression Results

| Dep. Variable      | price_scaled   | R-squared        | 0.517            |
|--------------------|----------------|-------------------|------------------|
| Model              | OLS            | Adj. R-squared    | 0.516            |
| Method             | Least Squares   | F-statistic       | 1158.            |
| Date               | Thu, 31 Oct 2024 | Prob (F-statistic) | 0.00           |
| Time               | 00:03:08       | Log-Likelihood     | -25794.          |
| No. Observations    | 14103          | AIC                | 5.162e+04        |
| Df Residuals       | 14089          | BIC                | 5.172e+04        |
| Df Model           | 13             | Covariance Type    | nonrobust        |

| Coefficient (coef) | Std Err        | t                 | P>|t|          | [0.025         | 0.975]         |
|---------------------|----------------|-------------------|----------------|----------------|----------------|
| const               | -79.2759       | 7.580             | -10.459        | 0.000          | -94.133        | -64.419        |
| bedrooms            | 0.3360         | 0.028             | 12.081         | 0.000          | 0.282          | 0.391          |
| baths               | 0.9000         | 0.031             | 29.207         | 0.000          | 0.840          | 0.960          |
| land_area           | 0.0061         | 0.000             | 12.415         | 0.000          | 0.005          | 0.007          |
| floor_area          | 0.0086         | 0.000             | 20.874         | 0.000          | 0.008          | 0.009          |
| nearby_supermarkets  | 0.0849        | 0.003             | 30.534         | 0.000          | 0.079          | 0.090          |
| nearby_stations     | 0.5742         | 0.015             | 38.088         | 0.000          | 0.545          | 0.604          |
| year_built          | 0.0392         | 0.004             | 10.413         | 0.000          | 0.032          | 0.047          |
| floor_level         | 0.0315         | 0.002             | 17.486         | 0.000          | 0.028          | 0.035          |
| facilities          | 0.0604         | 0.004             | 14.733         | 0.000          | 0.052          | 0.068          |
| Nonthaburi         | -0.9827        | 0.035             | -27.688        | 0.000          | -1.052         | -0.913         |
| Samut Prakan       | -0.8898        | 0.040             | -22.334        | 0.000          | -0.968         | -0.812         |
| Townhouse          | -1.6859        | 0.071             | -23.654        | 0.000          | -1.826         | -1.546         |
| Detached House     | -0.9954        | 0.114             | -8.763         | 0.000          | -1.218         | -0.773         |

| Omnibus             | 873.770        | Durbin-Watson     | 1.963            |
| Prob(Omnibus)      | 0.000          | Jarque-Bera (JB)  | 1396.598        |
| Skew                | 0.505          | Prob(JB)          | 5.40e-304       |
| Kurtosis            | 4.164          | Cond. No          | 1.20e+06        |

## Conclusion
This analysis demonstrates the significant impact of property features on pricing, with implications for buyers and investors. Understanding these factors enables more informed investment decisions in the real estate market.
"""

