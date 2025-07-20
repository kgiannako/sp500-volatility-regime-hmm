# 📊 Regime-Based Portfolio Strategies with Hidden Markov Models

This project explores the application of **Hidden Markov Models (HMMs)** to detect market regimes and inform systematic investment strategies.

We use both **daily** and **weekly S&P 500 returns** to model regime shifts, simulate investment strategies, and compare performance against traditional buy & hold.

---

## 🧩 Project Goals

- Model market regimes using HMM with financial return data.
- Compare daily vs weekly regime classifications.
- Test and evaluate regime-based investment strategies.
- Assess performance using key financial metrics:
  - Cumulative Returns
  - Sharpe Ratio
  - Sortino Ratio
  - Maximum Drawdown

---

## 🏗️ Methodology Summary

- **Regime Detection:**  
  Hidden Markov Models fitted on daily and weekly log returns, estimating distinct market states (e.g., calm, bullish, crisis).
  
- **Strategy Backtesting:**  
  Several systematic strategies were tested, including:
  - **Long in Calm Regime (State 0)**
  - **Long in Calm or Bullish Regimes (States 0 or 1)**
  - **Dynamic Exposure based on Detected State**
  - **Buy & Hold Baseline**

- **Performance Evaluation:**  
  Strategies compared on both daily and weekly data using risk-adjusted metrics.

---

## 📈 Practical Application — Using the Weekly HMM Model

### ✅ What Does the Model Do?
The model classifies the market into three regimes:
- **State 0 — Calm/Stable Market**
- **State 1 — Bullish/Speculative Market**
- **State 2 — Crisis/High-Risk Market**

---

### ✅ Suggested Strategy Summary

| Regime | Suggested Exposure | Rationale |
|--------|--------------------|-----------|
| **State 0 (Calm)** | **100% Long Equities** | Best risk-adjusted performance |
| **State 1 (Bullish)** | **100% Long** | Strong performance in weekly data |
| **State 2 (Crisis)** | **0% Exposure** | Avoid significant drawdowns |

---

### ✅ How to Use Practically

1. **Weekly Update** — Predict current market regime using recent weekly returns.
2. **Adjust Exposure** — Allocate as per detected regime.
3. **Monitor & Review** — Reassess performance periodically.

---

## 📊 Key Findings

- **Regime-aware strategies outperform Buy & Hold in both risk and return.**
- **Weekly model captures broader market phases better than daily model.**
- **Dynamic allocation strategies balance risk-adjusted performance with manageable drawdowns.**

---

## ⚖️ Disclaimer
This is an educational project.  
The strategies presented are for illustrative purposes and should not be considered financial advice.  

