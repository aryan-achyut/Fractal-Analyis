# AI-Driven Portfolio Optimization and Market Analysis

## Project Overview

This project implements advanced AI and data science techniques for portfolio optimization and market analysis, focusing on top tech stocks (AAPL, AMZN, GOOGL, META, MSFT). The goal is to design a portfolio that maximizes returns while managing risk through diverse optimization methods and market behavior analysis. We utilized Mean-Variance Optimization, Black-Litterman models, Sector Allocation, and Fractal Analysis for robust, data-backed investment strategies.

---

## Key Features

1. **Portfolio Optimization Techniques**:
   - Equal Weighting
   - Market Cap Weighting
   - Risk Parity
   - Sector Allocation
   - Mean-Variance Optimization
   - Black-Litterman
   - Minimum Variance

2. **Fractal Analysis & Stationarity Tests**:
   - Hurst Exponent to determine stock behavior: random walk or mean reversion.
   - Augmented Dickey-Fuller Test to check for stationarity.

3. **Backtesting & Risk Management**:
   - Volatility thresholds and optimized risk limits based on past economic data.
   - Integration of the `vix` library for volatility measures.

---

## Results Summary

### Portfolio Performance Metrics

| Optimization Strategy       | Annualized Return | Annualized Volatility | Sharpe Ratio |
|-----------------------------|-------------------|-----------------------|--------------|
| Equal Weighting             | 21.19%           | 20.34%                | 1.04         |
| Market Cap Weighting        | 19.75%           | 19.67%                | 1.00         |
| Risk Parity                 | 18.81%           | 18.53%                | 1.02         |
| Sector Allocation           | 35.15%           | 34.04%                | 1.03         |
| Mean-Variance Optimization  | 28.39%           | 22.81%                | 1.24         |
| Black-Litterman             | 24.16%           | 22.70%                | 1.06         |
| Minimum Variance            | 21.19%           | 20.34%                | 1.04         |

**Fractal Analysis Results**:
- **AAPL**: Random walk (Hurst Exponent = 0.536)
- **AMZN**: Random walk (Hurst Exponent = 0.507)
- **GOOGL**: Mean reversion tendency (Hurst Exponent = 0.479)
- **META**: Random walk (Hurst Exponent = 0.547)
- **MSFT**: Strong mean reversion (Hurst Exponent = 0.403)

**Stationarity (ADF Test Results)**:
All stocks show stationarity with p-values < 0.05, suggesting a stable mean and variance over time.

---

## Results and Insights

1. **High Sharpe Ratios**: Mean-Variance Optimization achieved the highest Sharpe Ratio (1.24), balancing risk and return effectively.
2. **Fractal Patterns**: Hurst Exponent revealed mean-reversion behavior in MSFT and GOOGL, while AAPL, AMZN, and META followed a random walk.
3. **Stationary Returns**: ADF tests confirmed stationarity, supporting stable mean and variance assumptions for returns.

---

## Future Work

- **Real-Time Economic Events Integration**: Incorporate real-time APIs to dynamically update economic data and adjust risk limits.
- **Advanced Machine Learning Models**: Use LSTM and reinforcement learning for more adaptive portfolio management.
- **Customizable Constraints**: Allow users to adjust constraints (e.g., max exposure per sector) for more tailored portfolio options.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

This project uses insights and techniques from financial research on portfolio optimization, with support from the Python libraries `yfinance`, `vix`, and `statsmodels`.

---

Happy Investing! 😊

---
