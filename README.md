# Multivariate Time Series Forecasting: Environmental & Chemical Data (IMD Pune)

## Overview  
This project explores **multivariate time series forecasting** on environmental and chemical data obtained from the **India Meteorological Department (IMD), Pune**.  
The goal was to analyze **temporal dependencies** between variables like rainfall, pH, conductivity, and ions, and apply advanced statistical models to capture volatility and interdependencies.  

This was a **group project** during my M.Tech coursework at **IIT Jodhpur**.  

---

## Objectives  
- Model temporal dependencies across **11 environmental and chemical parameters**.  
- Capture **volatility patterns** in pH and related variables using **GARCH models**.  
- Apply **VAR models** to understand dynamic interrelationships among multiple time series.  
- Validate models using **diagnostic tests and information criteria** (AIC, BIC, HQIC).  

---

## Dataset  
- Source: **IMD Pune**  
- Variables: Rainfall, pH, Conductivity, Ions, and other water-quality indicators (11 total).  
- Preprocessing:
  - Log transformations for variance stabilization.  
  - Stationarity checks (ADF tests).  
  - Correlation analysis across variables.  

---

## Methodology  

### 1. Exploratory Data Analysis  
- Visualized distributions, correlations, and temporal plots.  
- Identified heteroskedasticity and autocorrelation.  

### 2. GARCH Modeling (Volatility Analysis)  
- Applied **GARCH(2,1)** to log-transformed pH series.  
- Diagnostics: Box–Ljung and ARCH–LM confirmed ARCH effects.  
- Volatility plot revealed significant temporal fluctuations.  

### 3. VAR Modeling (Multivariate Dependencies)  
- Implemented **VAR(2)** to model relationships among 11 time series variables.  
- Estimated coefficients via **OLS regression**.  
- Analyzed AR(1) and AR(2) lag matrices to interpret inter-variable influence.  

---

## Key Results  

- **GARCH(2,1)** successfully captured volatility in pH data.  
  - AIC: -2.1158, BIC: -2.0551 → good model fit.  
- **VAR(2)** revealed strong dynamic relationships among environmental parameters.  
  - Rainfall and conductivity showed strong lagged dependencies.  
  - Some variables displayed weak or insignificant lag effects.  

---

## Takeaways  

- **Univariate models (ARIMA)** were insufficient for volatility → **GARCH provided a better fit**.  
- **Multivariate modeling (VAR)** allowed uncovering hidden relationships between chemical and environmental indicators.  
- Such models can inform **water quality monitoring and policy decisions**.  

---

## Repository Structure  

```markdown
time-series-forecasting-case-study/
│── presentation.pdf # Project PPT
│── report.pdf # Final project report
│── README.md # This file
```
---

```yaml
## Contributors  
- Sajad Ahmad Mir (M21MA207)  
- Himalaya (M21MA204)  
- Nasrat Jahan (M21MA205)  
- Raman Reshi (M21MA206)  
```

---

## References  
- Hamilton, J.D. (1994). *Time Series Analysis*.


