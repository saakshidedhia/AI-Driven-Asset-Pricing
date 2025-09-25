# 📈 AI-Driven Asset Pricing  

> **AI announcements don’t just change technology — they move markets.**  
This project analyzes how sentiment around AI-related announcements, especially **ChatGPT**, impacts the short-term returns of **technology-sector ETFs**.  

---

## 📂 Repository Structure  

- 📑 **AI_Driven_Asset_Pricing.pdf**  
  Full research paper with methodology, theoretical background, empirical results, and robustness checks.  

- 💻 **main_code.ipynb**  
  Jupyter Notebook implementing the analysis:  
  - Data preprocessing  
  - Event study framework for calculating **Cumulative Abnormal Returns (CAR)**  
  - Sentiment–return modeling with **OLS** and **ARIMAX**  
  - Visualizations of ETF prices, sentiment scores, and model outputs  

- 📊 **images/**  
  Visualizations and regression output screenshots (included below).  

- 📁 **Data Files**  
  Data files used in this project can be found here: [👉 Link to dataset]()  

---

## 📊 Key Visualizations  

### 1. ETF Returns vs Sentiment  
![ETF vs Sentiment](/SRC/1-ETFpricevsSentimentScores.png)  
*ETF price changes closely tracked sentiment scores during event windows.*  

---

### 2. OLS Regression Results  
![OLS Regression](/SRC/2-OLSRegressionResult.png)  
*OLS regression shows a positive and significant relationship between sentiment scores and 3-day CAR.*  

---

### 3. Overall Visualization  
![Overall Visualization](/SRC/3-OverallVisualization.png)  
*Scatter plot of sentiment vs CAR and distribution of CAR values across the sample.*  

---

### 4. ACF and PACF Analysis  
![ACF PACF](/SRC/4-CAR'sACFandPACF.png)  
*ACF and PACF plots helped determine ARIMAX model parameters.*  

---

### 5. ARIMAX(1,0,0) Results  
![ARIMAX(1,0,0)](/SRC/5-ARIMAXRegressionResult.png)  
*ARIMAX(1,0,0) confirms significance of sentiment and market factors in explaining CAR.*  

---

### 6. ARIMAX(0,0,0) Results  
![ARIMAX(0,0,0)](/SRC/6-ARIMAX_RegressionResult.png)  
*ARIMAX(0,0,0), essentially an OLS with exogenous factors, yields similar significance patterns.*  

---

## ⚙️ Tech Stack  

### 📊 Data Science & ML  
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/Numpy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=plotly&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Statsmodels](https://img.shields.io/badge/Statsmodels-333333?style=for-the-badge)
![ARCH](https://img.shields.io/badge/ARCH-E34F26?style=for-the-badge)

### 📓 Workflow  
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

---

## 🚀 How to Run  

1. **Clone the repository**  
   ```bash
   git clone <your-repo-link>
   cd <your-repo>
   ```
   ```bash
   jupyter notebook main_code.ipynb
   
## 📌 Results Summary

- ✅ **Sentiment is significant** → Higher AI sentiment scores correlate with higher ETF abnormal returns.
- 📉 **Volatility is not significant** → Market volatility does not strongly explain CAR.
- 📊 **Market performance matters** → ETF reactions are amplified by general NASDAQ performance.
- 🔍 **Robustness confirmed** → Findings hold across OLS, ARIMAX, and alternative specifications.

## 📖 Citation
If you use this work, please cite the research report:

_Saakshi Dedhia, Xin Qin, Yaxi Chen, and Mao Li (2025). AI Driven Asset Pricing: The Impact of ChatGPT and AI Announcements on Tech Stocks (ETFs). ECON 515 Research Paper.
_
