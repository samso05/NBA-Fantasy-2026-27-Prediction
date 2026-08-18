# NBA Fantasy Points & VORP Projection Pipeline 🏀

An end-to-end Machine Learning pipeline using **XGBoost** to forecast season-long ESPN Fantasy Points Per Game (FPTS/G) and Value Over Replacement Player (VORP) for 16-team fantasy leagues.

## 📌 Project Overview
- **Data Engine**: Processes multi-year player game logs using `pyarrow` and `pandas`.
- **Feature Engineering**: Calculates 1-, 2-, and 3-year lagged performance features across scoring efficiency, usage, and volume.
- **Model**: Gradient boosted decision trees (`XGBRegressor`) evaluated via cross-season backtesting.
- **Output**: Generates a customized 16-team Draft Board formatted in Excel with position-based replacement baselines.
