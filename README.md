# Predicting Monthly Passenger Air Traffic in Brazil
## Overview
This project develops a robust forecasting model for total monthly passenger air traffic in Brazil, designed to support strategic airport expansion and infrastructure investment planning through 2028. Using the CRISP-DM methodology and over 22 million flight records from Brazil's National Civil Aviation Agency (ANAC), the analysis delivers a 36-month forecast with a Mean Absolute Percentage Error (MAPE) below 20%.

## Business Objective
The Ministry of Infrastructure requires precise, data-driven forecasts of passenger volumes to guide capacity planning decisions. The project targets:
- Forecast horizon: 36 months
- Target metric: Monthly passenger traffic
- Performance requirement: MAPE below 20%

## Dataset
The analysis leverages ANAC's air transport microdata, covering:
- 22.1 million individual records
- 111 attributes per record
- 25 years of data (2000–2025)
- All domestic and international flights operated by Brazilian and foreign carriers

## Results
### Selected Model: SARIMAX
The SARIMAX model was selected for production stability, providing verified prediction intervals for 2026 infrastructure capacity planning: it achieved 6–17% MAPE.

### Seasonality and Structural Breaks
- Annual Seasonality: Clear, stable annual pattern with predictable peaks.
- COVID-19: Sharp decline in early 2020; international traffic collapsed almost entirely.
- Domestic Lead: Domestic traffic recovered faster and exceeded pre-pandemic levels earlier than international routes.
- Broken Correlations: Historically strong correlation between passenger and cargo traffic disappeared post-pandemic.
- Non-revenue Stability: Ratio of free to paid passenger tickets remains stable at approximately 0.02 annually.

## Forecast Risks
External shocks create uncertainty, requiring regular model retraining to ensure forecast accuracy.
