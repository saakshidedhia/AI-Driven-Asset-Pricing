# AI-Driven Asset Pricing

This repository contains the research and implementation for the project **"AI Driven Asset Pricing: The Impact of ChatGPT and AI Announcements on Tech Stocks (ETFs)"**.  
It explores how sentiment around AI-related announcements, especially those involving ChatGPT, affects the short-term returns of technology-sector ETFs.

---

## 📂 Contents

- **AI_Driven_Asset_Pricing.pdf**  
  Full research paper describing methodology, theoretical background, empirical results, and robustness checks.

- **main_code.ipynb**  
  Jupyter Notebook implementing the analysis, including:
  - Data preprocessing  
  - Event study framework for calculating Cumulative Abnormal Returns (CAR)  
  - Sentiment–return modeling with OLS and ARIMAX  
  - Visualization of ETF prices, sentiment scores, and model outputs  

- **Data Files**  
  Data files used in this project can be found here: [Link to dataset]()

- **images/**  
  Visualizations and regression output screenshots included in this README.

---

## 📊 Visualizations

### ETF Returns vs Sentiment
![ETF vs Sentiment](/SRC/1-ETFpricevsSentimentScores.png)  
*ETF price changes closely tracked sentiment scores during event windows.*

---

### OLS Regression Results
![OLS Regression](/SRC/2-OLSRegressionResult.png)  
*OLS regression shows a positive and significant relationship between sentiment scores and 3-day CAR.*

---

### Overall Visualization
![Overall Visualization](/SRC/3-OverallVisualization.png)  
*Scatter plot of sentiment vs CAR and distribution of CAR values across the sample.*

---

### ACF and PACF Analysis
![ACF PACF](/SRC/4-CAR'sACFandPACF.png)  
*ACF and PACF plots helped determine ARIMAX model parameters.*

---

### ARIMAX(1,0,0) Results
![ARIMAX(1,0,0)](/SRC/5-ARIMAXRegressionResult.png)  
*ARIMAX(1,0,0) confirms significance of sentiment and market factors in explaining CAR.*

---

### ARIMAX(0,0,0) Results
![ARIMAX(0,0,0)](/SRC/6-ARIMAX_RegressionResult.png)  
*ARIMAX(0,0,0), essentially an OLS with exogenous factors, yields similar significance patterns.*

---

## ⚙️ Requirements

The notebook is written in **Python 3** and uses the following main libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `statsmodels`
- `arch` (for GARCH models)
- `scikit-learn`
- `jupyter`

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone <your-repo-link>
   cd <your-repo>
