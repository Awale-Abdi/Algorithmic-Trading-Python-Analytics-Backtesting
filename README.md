<h1 align="center">Predictive Analytics & Statistical Modeling | Data-Driven Portfolio Analysis with Python</h1>

This project showcases an **end-to-end predictive analytics and statistical analysis workflow** built using approximately **15 million financial data points across 1.87 million historical stock-price records and more than 500 companies**. I developed it to demonstrate large-scale data preparation, exploratory data analysis, feature engineering, statistical analysis, systematic strategy development, simulation, backtesting, and quantitative performance evaluation.

Although the project uses **S&P 500 financial market data** as its case study, the analytical techniques I apply, such as exploratory data analysis, statistical analysis, segmentation, feature engineering, random-sampling simulation, benchmark comparison, and systematic experimentation, are broadly transferable to operations, manufacturing, healthcare, insurance, marketing, risk analytics, and other data-driven fields.

Using **Python**, **Pandas**, **NumPy**, and statistical and visualization techniques, I transformed large-scale structured data into an analytical framework for identifying patterns, evaluating alternatives, testing a data-driven strategy, and measuring its performance against a defined benchmark.

The resulting workflow demonstrates how exploratory analysis can progress systematically from raw data preparation and pattern discovery through hypothesis development, experimentation, validation, and decision-support insights.

## 💼 Analytical Goals

The project focuses on applying data science, statistical analysis, and systematic experimentation to determine whether historical patterns can be used to develop and evaluate a robust data-driven strategy.

The primary goals were to:

- Prepare and analyze large-scale structured datasets
- Explore historical patterns across companies and sectors
- Evaluate price behavior, returns, volatility, and risk characteristics
- Identify meaningful analytical segments and comparative patterns
- Develop a rule-based strategy from exploratory findings
- Test the strategy through repeated random-sampling simulations
- Benchmark performance against the S&P 500
- Evaluate results using quantitative risk and performance metrics
- Translate analytical findings into actionable decision-support insights

## 🏗️ Solution Architecture

#### Workflow

```text
Large-Scale Structured Datasets
        ↓
Data Preparation & Cleaning
        ↓
Exploratory Data Analysis
        ↓
Segmentation & Feature Engineering
        ↓
Statistical & Volatility Analysis
        ↓
Sector-Level Comparative Analysis
        ↓
Strategy Development
        ↓
Random-Sampling Simulation
        ↓
Quantitative Backtesting
        ↓
Benchmark Comparison
        ↓
Risk & Performance Evaluation
        ↓
Analytical Interpretation
```

#### Data

- **Dataset:** S&P 500 Company, Stock Price, and Index Data
- **Companies:** 503 S&P 500 company records
- **Stock Price Records:** ~1.87 million historical observations
- **S&P 500 Index Records:** 2,516 observations
- **Historical Analysis Period:** 2010–2024
- **Data Formats:** CSV and Parquet
- **Primary Data:** Historical stock prices, trading volume, company and sector metadata, and S&P 500 index values

The analysis uses three complementary datasets:

```text
sp500_companies.csv
sp500_index.csv
sp500_stocks.parquet
```

Together, these datasets provide company-level attributes, sector classifications, historical market prices, trading activity, and benchmark index performance.

#### Data Preparation

Performed large-scale data preparation by:

- Loading and validating multiple structured datasets
- Converting date fields into appropriate time-series formats
- Standardizing numeric variables for analysis
- Identifying and handling missing values
- Detecting and removing anomalous trading-volume records
- Integrating company metadata with historical stock-price data
- Preparing structured datasets for downstream statistical analysis

#### Exploratory Data Analysis

Conducted exploratory analysis to evaluate:

- Historical stock-price distributions
- Trading-volume characteristics
- Descriptive statistical patterns
- Price variability
- Company-level behavior
- Market-wide distributions
- Potential analytical segments and investment opportunities

Stocks were segmented into price-based cohorts to compare behavioral differences across the dataset and provide a structured basis for deeper analysis.

#### Feature Engineering & Segmentation

Engineered analytical features and classifications including:

- Daily returns
- Average closing prices
- Price-based cohorts
- Stock-level volatility
- Volatility cohorts
- Sector classifications
- Sector-level performance measures

These features allowed the analysis to progress from individual stock observations toward broader comparative patterns across companies and sectors.

#### Statistical & Sector Analysis

Conducted deeper comparative analysis by:

- Integrating stock-price data with company and sector metadata
- Comparing average closing prices across sectors
- Measuring volatility using the standard deviation of daily returns
- Examining the distribution of price cohorts within sectors
- Segmenting securities into low, medium, and high volatility groups
- Comparing risk characteristics across market segments
- Identifying sectors displaying favorable combinations of historical performance and stability

The exploratory and statistical findings were then used to guide the development of the final strategy.

#### Strategy Development

Based on the preceding analysis, the **Healthcare sector** was selected for systematic testing due to its observed combination of historical performance, volatility characteristics, and representation across price cohorts.

A rule-based experimental strategy was developed to compare randomly constructed healthcare portfolios against the S&P 500 benchmark over the historical period.

#### Simulation & Backtesting

The strategy was evaluated through **1,000 random-sampling iterations**.

During each iteration:

- Five healthcare stocks were randomly selected without replacement
- Historical daily returns were calculated for the selected portfolio
- Portfolio returns were aggregated across the selected companies
- Cumulative portfolio performance was calculated
- Equivalent S&P 500 benchmark performance was calculated
- Final portfolio values were compared
- Winning and losing iterations were recorded

Repeating this process across 1,000 independently sampled portfolios provided a more robust evaluation than relying on the performance of a single hand-selected portfolio.

#### Performance Evaluation

Performance was evaluated using:

- Compound Annual Growth Rate (CAGR)
- Sharpe Ratio
- Sortino Ratio
- Maximum Drawdown
- Annualized Volatility
- Calmar Ratio
- Benchmark Outperformance Frequency
- Average Outperformance
- Average Underperformance
- Cumulative Portfolio Value

Results were aggregated across the simulation framework and compared directly with the S&P 500 benchmark.

## 📊 Analytical Insights

#### Portfolio Performance

Across **1,000 random-sampling iterations**, the healthcare strategy demonstrated strong historical performance relative to the S&P 500 benchmark.

Average performance metrics were:

| Metric | Healthcare Portfolio | S&P 500 |
|---|---:|---:|
| CAGR | **13.18%** | 11.26% |
| Sharpe Ratio | **0.80** | 0.70 |
| Sortino Ratio | **1.06** | 0.85 |
| Maximum Drawdown | **-29.18%** | -33.92% |
| Volatility | **17.60%** | 17.85% |
| Calmar Ratio | **0.45** | 0.33 |

The healthcare portfolios:

- Outperformed the S&P 500 in approximately **63% of the 1,000 iterations**
- Outperformed by approximately **42.53%** of the benchmark's average final portfolio value during winning iterations
- Underperformed by approximately **22.20%** during losing iterations
- Produced a higher average CAGR than the benchmark
- Generated stronger Sharpe and Sortino ratios
- Experienced a smaller maximum drawdown
- Produced a stronger Calmar ratio

#### Quantitative Analysis

- Sector-level segmentation revealed meaningful differences in historical price behavior and volatility.
- Volatility analysis provided additional information beyond raw price performance.
- Risk-adjusted metrics provided a more complete evaluation than returns alone.
- Repeated random sampling reduced dependence on the performance of any single manually selected portfolio.
- Benchmark comparison provided a consistent baseline for strategy evaluation.
- The simulation demonstrated how systematic experimentation can evaluate the robustness of an analytical hypothesis across varying samples.

## ⚠️ Project Limitations

- Historical performance does not guarantee future results.
- The analysis evaluates historical market behavior and should not be interpreted as investment advice.
- Randomly sampled portfolios were limited to five healthcare stocks per iteration.
- The strategy does not incorporate transaction costs, taxes, slippage, or portfolio rebalancing costs.
- Sector membership and company characteristics can change over time.
- The analysis does not explicitly control for survivorship bias.
- The strategy is rule-based rather than a trained predictive machine learning model.
- Results depend on the historical period and datasets used.

These limitations mean the results should be interpreted as a demonstration of **data-driven strategy development, simulation, and experimental evaluation**, rather than evidence that the historical strategy will necessarily outperform in future markets.

## 📈 Analytical Recommendations

- Evaluate analytical strategies using both absolute and risk-adjusted performance measures.
- Use repeated sampling and experimentation rather than relying on individual observations or manually selected cases.
- Compare analytical strategies against clearly defined benchmarks.
- Incorporate volatility and downside-risk measures when evaluating performance.
- Extend the framework across additional sectors and portfolio sizes to test the robustness of observed patterns.
- Introduce rolling-window or out-of-sample testing to evaluate performance across different historical periods.
- Incorporate additional features and predictive models to test whether more sophisticated approaches improve performance.
- Regularly reevaluate strategies as new data becomes available.

## 🛠️ Technical Skills Demonstrated

#### Programming

- Python
- Pandas
- NumPy

#### Data Science & Analytics

- Large-Scale Dataset Processing
- Data Cleaning
- Data Transformation
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Integration
- Segmentation
- Comparative Analysis
- Systematic Experimentation

#### Statistical Analysis

- Descriptive Statistics
- Distribution Analysis
- Daily Return Analysis
- Standard Deviation
- Volatility Analysis
- Risk Analysis
- Quantitative Performance Evaluation

#### Predictive & Experimental Analytics

- Rule-Based Strategy Development
- Random-Sampling Simulation
- Quantitative Backtesting
- Benchmark Comparison
- Repeated Experimental Evaluation
- Performance Validation

#### Data Visualization

- Matplotlib
- Seaborn
- Plotly
- Interactive Visualization
- Distribution Visualization
- Comparative Performance Visualization

#### Quantitative Analytics

- CAGR
- Sharpe Ratio
- Sortino Ratio
- Maximum Drawdown
- Annualized Volatility
- Calmar Ratio
- Cumulative Return Analysis
- Portfolio Performance Analysis
- Risk-Adjusted Performance Analysis

#### Development Environment

- Jupyter Notebook
- Git
- GitHub

## 💡 What This Project Demonstrates

This project demonstrates the ability to independently design and execute an end-to-end analytical solution using large-scale structured datasets.

Specifically, it showcases proficiency in:

- Preparing and transforming large datasets for analysis
- Conducting exploratory and statistical analysis
- Engineering analytical features from raw observations
- Identifying patterns through segmentation and comparative analysis
- Developing hypotheses and rule-based strategies from analytical findings
- Designing repeated random-sampling experiments
- Backtesting analytical strategies against defined benchmarks
- Evaluating outcomes using multiple quantitative performance metrics
- Developing static and interactive data visualizations
- Translating complex quantitative results into actionable decision-support insights

As stated prior, although financial market data provides the case study, the underlying workflow of **data preparation → exploratory analysis → feature engineering → segmentation → hypothesis development → simulation → validation → performance evaluation → decision support** is broadly transferable across Data Science, Business Analytics, operations, manufacturing, healthcare, insurance, marketing, risk analysis, experimentation, and a wide range of other data-driven fields.

## 📁 Repository Structure

```text
Predictive-Analytics-Statistical-Modeling-Portfolio-Analysis-Python/
│
├── Datasets/
│   ├── sp500_companies.csv
│   ├── sp500_index.csv
│   └── sp500_stocks.parquet
│
├── Outputs/
│   ├── high_price_distribution.jpg
│   ├── interactive_backtest_plot.html
│   ├── low_price_distribution.jpg
│   ├── middle_price_distribution.jpg
│   ├── sector_avg_closing_price_distribution.jpg
│   ├── sector_volatility_cohort.jpg
│   └── sector_volatility_price_cohort.jpg
│
├── Python Notebook/
│   └── Data-Driven Investment Strategy - Analyzing Financial Data for Portfolio Optimization.ipynb
│
├── .gitattributes
│
└── README.md
```

**Datasets**

Contains the three datasets required to reproduce the analysis:

- S&P 500 company and sector metadata
- Historical S&P 500 index values
- Historical individual stock-price data

**Outputs**

Contains the static and interactive visualizations generated throughout the exploratory, sector, volatility, and backtesting analyses.

**Python Notebook**

Contains the complete analytical workflow from data preparation through exploratory analysis, statistical analysis, strategy development, simulation, backtesting, and final interpretation.

## 📋 Replicating the Project

#### Clone the Repository

```bash
git clone https://github.com/Awale-Abdi/Algorithmic_Trading_Healthcare_Portfolio.git
cd Algorithmic_Trading_Healthcare_Portfolio
```

#### Required Data

All datasets required to reproduce the project are included in:

```text
Datasets/
```

The analysis requires:

```text
sp500_companies.csv
sp500_index.csv
sp500_stocks.parquet
```

#### Open the Notebook

Navigate to:

```text
Python Notebook/
```

Then open:

```text
Data-Driven Investment Strategy - Analyzing Financial Data for Portfolio Optimization.ipynb
```

#### Required Python Libraries

The analysis uses:

```text
pandas
numpy
matplotlib
seaborn
plotly
pyarrow
```

`pyarrow` or another compatible Parquet engine is required to load the stock-price dataset.

#### Run the Analysis

Execute the notebook sequentially to reproduce:

- Data preparation and cleaning
- Exploratory Data Analysis (EDA)
- Price-cohort segmentation
- Feature engineering
- Sector-level comparative analysis
- Daily-return calculations
- Volatility analysis
- Strategy development
- 1,000-iteration random-sampling simulation
- Quantitative backtesting
- S&P 500 benchmark comparison
- Risk and performance evaluation
- Static and interactive visualizations

Generated analytical outputs can then be compared with the files contained in:

```text
Outputs/
```

## 📬 Contact Me

**Email**

Awaleiabdi@outlook.com

**LinkedIn**

https://www.linkedin.com/in/awale-abdi
