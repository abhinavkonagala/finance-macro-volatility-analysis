# Macroeconomic Indicators & Market Volatility Analysis
**Investment Strategy Development Through Quantitative Risk Modeling**

## Executive Summary
**Bottom Line Up Front**: Current market environment supports cautious bullish positioning with 75% equity allocation, reduced from typical 85% due to overbought technical conditions (RSI: 71.2). Predicted monthly volatility: 2.5% with 95% VaR at -4.2%.

**Business Impact Delivered**:
- Portfolio managers receive tactical allocation signals with quantified risk parameters
- Risk teams gain enhanced volatility predictions (1.5% accuracy vs 3-4% industry standard)  
- Client advisory teams access clear risk-return scenarios with historical validation
- Investment committee receives regime-based allocation framework reducing drawdown risk

## Key Findings

| Metric | S&P 500 | NASDAQ | Insight |
|--------|---------|---------|---------|
| Annual Return | 7.2% | 9.0% | NASDAQ premium comes with 43% higher volatility |
| Sharpe Ratio | 0.340 | 0.324 | S&P 500 delivers superior risk-adjusted returns |
| Max Drawdown | -52.6% | -75.0% | Diversification reduces tail risk by 22 percentage points |
| 95% VaR | -8.0% | -10.1% | S&P 500 monthly loss threshold 2.1% lower |

**Market Regime Analysis**: Bull/Low Volatility conditions occur 51% of time and generate optimal risk-adjusted returns. Current regime classification supports equity overweight with tactical caution.

## Investment Recommendations

### Portfolio Allocation
- **S&P 500**: 55% (core broad market exposure)
- **NASDAQ**: 20% (growth component with volatility awareness)  
- **Bonds**: 15% (defensive allocation for rate environment)
- **Cash**: 10% (tactical reserve for opportunities)

### Risk Management Framework
- **Monthly VaR Estimate**: -4.2% (95% confidence level)
- **Rebalancing Triggers**: 5% allocation drift or regime classification changes
- **Position Sizing**: Low volatility environment supports normal position sizes
- **Downside Protection**: Stop-loss protocols activated if predicted volatility exceeds 6%

### Rationale
Allocation reflects overbought technical conditions requiring defensive positioning despite supportive Bull/Low Vol regime. 10% cash reserve enables opportunistic rebalancing when RSI normalizes below 70.

## Technical Implementation

### Data Architecture
**Sources**: Federal Reserve Economic Data (FRED), Yahoo Finance API  
**Coverage**: 307 monthly observations (2000-2025)  
**Indicators**: Unemployment rate, inflation, federal funds rate, Treasury yields, VIX, market indices  
**Quality Controls**: Timezone standardization, missing value treatment, outlier detection

### Analytical Framework

**Phase 1: Data Foundation**
- Multi-source data integration (FRED, Yahoo Finance)
- Timezone standardization and frequency alignment
- Quality assurance and missing value treatment
- Data validation and outlier detection

**Phase 2: Financial Analysis**
- Correlation matrices and statistical relationships
- Risk metrics (VaR, Sharpe ratios, drawdowns)
- Market regime classification (Bull/Bear × High/Low Vol)
- Technical indicator calculations

**Phase 3: Predictive Modeling**
- Random Forest volatility prediction models
- Feature engineering with lagged variables
- Cross-validation and performance testing
- Model interpretation and feature importance

**Phase 4: Investment Strategy**
- Portfolio optimization and allocation recommendations
- Scenario analysis and stress testing
- Executive reporting and visualization
- Risk management framework development

### Model Performance
- **Volatility Prediction**: Random Forest achieving 1.54% Mean Absolute Error
- **Top Predictors**: 3-month moving average (30.9%), lagged returns (7.4%), VIX indicators (16.1%)
- **Regime Classification**: Bull/Bear identification with volatility overlay
- **Backtesting**: Strategy framework tested across multiple market cycles

## Historical Strategy Performance
**Total Return Comparison**: Buy & Hold (363.3%) vs Tactical Strategy (210.1%)  
**Key Insight**: Simple buy-and-hold outperformed tactical timing by 153 percentage points, demonstrating market timing difficulty and validating disciplined allocation approach over reactive strategies.

## Repository Structure

- **01_Data_Collection_Validation.ipynb** - Multi-source data integration and quality assurance
- **02_EDA_Financial_Metrics.ipynb** - Risk metrics and correlation analysis  
- **03_Time_Series_Risk_Modeling.ipynb** - Predictive modeling and technical indicators
- **04_Executive_Dashboard.ipynb** - Investment strategy and reporting
- **README.md** - Project documentation
- **requirements.txt** - Python environment setup

## Technologies Used
**Core**: Python, pandas, numpy, scikit-learn  
**Financial Data**: yfinance, pandas-datareader (FRED API)  
**Analysis**: scipy, statsmodels for statistical modeling  
**Visualization**: matplotlib, seaborn for professional charts  
**Machine Learning**: Random Forest regression for volatility forecasting

## Methodology Highlights
- **Risk Metrics**: Industry-standard VaR, Expected Shortfall, Maximum Drawdown calculations
- **Correlation Analysis**: Pearson correlation matrices with statistical significance testing
- **Technical Analysis**: RSI, moving averages, Bollinger Bands for market timing
- **Regime Classification**: Bull/Bear markets with volatility overlays for tactical allocation
- **Predictive Modeling**: Supervised learning with lagged features and cross-validation

## Limitations & Assumptions
- Analysis focused on US markets; international diversification not modeled
- Risk-free rate assumed at 2% for Sharpe ratio calculations  
- Transaction costs simplified in backtesting scenarios
- Historical relationships may not persist in changing market structures

## Data Access
Raw datasets are not included in this repository due to size constraints. The notebooks automatically download data from:
- Federal Reserve Economic Data (FRED) API
- Yahoo Finance API
- Original Kaggle dataset reference provided in notebook 01

---
## Contact
- **Name**: Abhinav Konagala
- **LinkedIn**: [linkedin.com/in/abhinav-konagala](https://www.linkedin.com/in/abhinav-konagala/)
- **Email**: [akdhpo+work@pm.me](mailto:akdhpo+work@pm.me)
