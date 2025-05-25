<h1 align="center">Data-Driven Investment Strategy – Analyzing Financial Data for Portfolio Optimization</h1>

This project applies Data Science techniques to financial data—processing up to ~14.96 million data points from 503 companies & 1.86M stock records using **Python**—to design a profitable and robust investment strategy. By analyzing price behavior, volatility, and sector trends within the S&P 500, it identifies key patterns for optimal portfolio selection and aims to demonstrate how data-driven insights can enhance investment decision-making and portfolio performance.

---

## 🎯 Objective

To apply data science techniques to evaluate and backtest an investment strategy rooted in sector-based insights. This project aims to optimize portfolio composition through rigorous analysis and benchmark performance against the S&P 500.

Key goals:
- Clean, transform, and analyze high-volume financial data  
- Evaluate sector volatility and price trends  
- Develop a rule-based investment strategy  
- Backtest and benchmark strategy performance  
- Assess risk-adjusted returns using financial metrics  
- Present clear findings through visualizations and summary  

---

## ⚙️ Structure of Workflow

- **Data Preparation** – Cleaning, transforming, and structuring stock price and sector data  
- **Exploratory Data Analysis (EDA)** – Investigating stock distributions, trends, and initial volatility insights  
- **Deeper Data Analysis** – Evaluating price behavior, volatility, and sector distributions to identify strong investment candidates  
- **Backtesting Chosen Strategy** – Implementing a rule-based investment approach and benchmarking it against the S&P 500  
- **Conclusion** – Summarizes the chosen strategy's performance and what it says about a data-driven approach to portfolio optimization  

---

## 📊 Tools & Techniques Used

- **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`  
- **Financial Metrics:** CAGR, Sharpe Ratio, Sortino Ratio, Max Drawdown, Volatility, Calmar Ratio  
- **Backtesting Methodology:** Simulated healthcare portfolio selections with 1,000 iterative comparisons against the S&P 500 (2010–2024)  

---

## 📈 Key Findings

The healthcare sector emerged as a strong investment choice due to its balance of stability and returns. The backtested portfolio outperformed the S&P 500 in ~60% of iterations run while limiting downside risks. Even when underperforming, the portfolio only lagged behind the S&P by ~20% on average, but when winning, it exceeded it by ~40% on average. Risk-adjusted metrics like Sharpe and Sortino ratios confirmed the portfolio’s superior risk-return tradeoff. This balance of higher returns with controlled risk underscores healthcare as a strategic investment sector and highlights the value of applying data science to portfolio design.

---

## 🧾 Project Setup

### 1. Clone the Repository
```bash
git clone https://github.com/Awale-Abdi/Algorithmic_Trading_Healthcare_Portfolio

### 2. Prepare Datasets

Ensure the following datasets are present in your working directory:

- `sp500_companies.csv`  
- `sp500_index.csv`  
- `sp500_stocks.parquet`  

These files are loaded via relative paths and are required for the notebook to run correctly.

---

### 3. Run the Jupyter Notebook

Launch the notebook environment and execute:

- `Data-Driven Investment Strategy - Analyzing Financial Data for Portfolio Optimization.ipynb`

---

## 📬 Contact Me

For questions or collaboration, reach out via:

- 📧 Awaleiabdi@outlook.com  
- 💼 [LinkedIn](https://www.linkedin.com/in/awale-abdi/)
