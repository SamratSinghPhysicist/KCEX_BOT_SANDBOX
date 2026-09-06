# 🚀 KCEX Quantitative Trading & Dual-Feed Backtesting Suite (Sandbox)

> **Monorepo Structure**: Autonomous Quantitative Research, Microstructure Forensics, and High-Fidelity Execution Engines for KCEX Futures.

---

## 📁 Repository Organization

```
(COPY-SandBoxed) KCEX/
├── ResearchV1/                # Phase 1 & 2: Baseline quantitative backtests, initial strategy exploration & execution engines
│   ├── AI_ANALYSIS/           # Initial LLM forensics and trade breakdown reports
│   ├── BACKTESTER/            # Baseline backtesting engine and reports
│   ├── kcex/                  # KCEX REST & WebSocket API clients
│   ├── strategies/            # Strategy signal generators
│   └── semi_auto_trader.py    # Semi-automated execution harness
│
├── ResearchV2/                # Phase 2.1 & 2.2: Definitive millisecond tick engine, tick ratchet & Monte Carlo suite
│   ├── AI_ANALYSIS/           # Master Overnight Research Dossier V2.2 & synthesis
│   ├── BACKTESTER/            # High-fidelity millisecond tick backtesting engine
│   ├── research_v2_2/         # Vectorized empirical research scripts (Tracks 1, 2, 4, 5)
│   ├── kcex/                  # KCEX trading client & order manager
│   ├── strategies/            # Dynamic indicators (StochRSI, EMA Crossover, Regime Filters)
│   └── KCEX_RESEARCH_V2_2_COMPLETE_PACKAGE/ # Master deliverable package and presets
│
├── .github/workflows/         # Cloud GitHub Actions workflows for automated high-volume backtesting
├── .gitignore                 # Monorepo git exclusion rules
└── README.md                  # Project index and architecture overview
```

---

## 🔬 Research Tracks & Scientific Breakthroughs (V2.2)

1. **Track 1 (Slippage Degradation Curves)**:
   - Analytical derivation of Critical Slippage Threshold: $S_{max} = \frac{W \cdot \text{TP} - (1 - W) \cdot \text{SL}}{2 - W}$.
   - Asymmetric reward-to-risk setups ($10\text{t}/2\text{t}$ and $5\text{t}/2\text{t}$ + Ratchet) survive adverse friction, while tight symmetric scalps ($2\text{t}/2\text{t}$) collapse.
2. **Track 2 (Micro-Excursion Tick Ratchet)**:
   - 192-parameter grid search across 47,812 trades identified optimal parameters: Trigger $+1.0\text{t}$, Stall $10.0\text{s}$, Tighten $-1.0\text{t}$, Breakeven $+2.5\text{t}$.
   - Sortino Ratio elevated from $7.21$ to **$538.78$**, Net PnL expanded by **+175.1%** (`+$4.8692 USDT`), Max Drawdown halved to **`-0.014%`**.
3. **Track 4 (Regime Fading vs Breakout Momentum)**:
   - In Choppy regimes ($\text{CHOP} > 55$ / $\text{ADX} < 20$), Inverted Fading achieves **+61.4% to +84.1% higher Profit Factor** than Direct momentum.
4. **Track 5 (Walk-Forward OOS & 10,000 Monte Carlo Bootstrap)**:
   - 100% Out-of-Sample Survival (Profile 1 IS `+$2.18` $\to$ OOS `+$2.69`, RDI = 1.15).
   - Across 10,000 bootstrap resamplings, empirical Probability of Ruin is **`0.0000%`**.

---

## 🛠️ Quick Start & Running Backtests

```bash
# Run local high-fidelity tick backtest (V2.2 engine)
cd ResearchV2
python BACKTESTER/run_backtest.py --symbol DOGE_USDT --timeframe 1m --strategy STOCH_RSI --stoch-preset FAST_SCALP --ticks --invert-signal
```
