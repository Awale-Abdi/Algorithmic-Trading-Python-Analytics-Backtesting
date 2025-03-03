# Data-Driven Investment Strategy: Analyzing Financial Data for Portfolio Optimization

### **Overview**

This project applies Data Science techniques to financial data to design a profitable and robust investment strategy. By analyzing price behavior, volatility, and sector trends within the S&P 500, it identifies key patterns for optimal portfolio selection and aims to demonstrate how data-driven insights can enhance investment decision-making and portfolio performance.

### **Structure of Workflow**

- **Data Preparation:** Cleaning, transforming, and structuring stock price and sector data.
- **Exploratory Data Analysis (EDA):** Investigating stock distributions, trends, and initial volatility insights.
- **Deeper Data Analysis:** Evaluating price behavior, volatility, and sector distributions to identify strong investment candidates.
- **Backtesting Chosen Strategy:** Implementing a rule-based investment approach and benchmarking it against the S&P 500.
- **Conclusion:** Wrapping  & evaluation of the chosen strategy's performance and what it says about a data-driven approach to portfolio optimization.

### **Tools & Techniques Used**

- **Libraries:** pandas, numpy, matplotlib, seaborn, plotly
- **Financial Metrics:** CAGR, Sharpe Ratio, Sortino Ratio, Max Drawdown, Volatility, Calmar Ratio
- **Backtesting Methodology:** Simulated healthcare portfolio selections with 1,000 iterative comparisons against the S&P 500 (2010-2024)

### **Key Findings**

The healthcare sector emerged as a strong investment choice due to its balance of stability and returns. The backtested portfolio outperformed the S&P 500 in ~60% of iterations run while limiting downside risks. Even when underperforming, the portfolio only lagged behind the S&P by ~20% on average, but when winning, it exceeded it by ~40% on average. Risk-adjusted metrics like Sharpe and Sortino ratios confirmed the portfolio’s superior risk-return tradeoff. This balance of higher returns with controlled risk underscores healthcare as a strategic investment sector and highlights the value of applying data science to portfolio design.

### **Future Improvements**

- Implement Monte Carlo simulations to model risk scenarios.

- Explore alternative asset classes (bonds, commodities, cryptocurrencies).

- Apply machine learning models for predictive insights and for optimizing the strategy's performance.

### **How to Use**

#### **1. Clone the Repository**
```sh
git clone https://github.com/Awale-Abdi/Algorithmic_Trading_Healthcare_Portfolio
```
#### 2. Have the Datasets present in your working directory

The analyses rely on the following three datasets being present in your working directory:

- sp500_companies.csv
- sp500_index.csv
- sp500_stocks.parquet
  
You must have all these files present in your working directory for the Python Notebook to run without errors. They are loaded via relative paths, so as long as they are in your working directory, everything should work fine.

#### **3. Run the Python Notebook**
Run the Jupyter Notebook environment, have the prior outlined datasets present in your working directory and execute the following notebook:

- Data-Driven Investment Strategy - Analyzing Financial Data for Portfolio Optimization.ipynb

### **Contact Me**

For questions or collaboration, reach out via:

- Awaleiabdi@outlook.com

- [GitHub](https://github.com/Awale-Abdi)

- [LinkedIn](https://www.linkedin.com/in/awale-abdi/)

