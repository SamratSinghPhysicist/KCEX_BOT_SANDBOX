# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:11:12 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.2062 USDT` | `₹19.48` | `+194.57%` |
| **Net Realized PnL** | **`+0.1362 USDT`** | **`₹+12.86`** | **`+194.57% Net ROI`** |
| **Gross Profit** | `+0.9234 USDT` | `₹87.22` | Total positive trade returns |
| **Gross Loss** | `-0.7872 USDT` | `₹74.35` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.17`** | — | Profitable |
| **Win / Loss Payoff** | `0.37` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0380 USDT` | `₹3.59` | **`-26.40%` Peak-to-Trough** |
| **Win Rate** | **`75.78%`** | — | `1539 Wins / 492 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `5.53` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `3.27` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `7.37` | — | Net ROI divided by Max Drawdown |

---

## 🛠️ Complete Configuration & Settings Used

### Strategy & Market Setup
| Configuration Setting | Value | Operational Details |
| :--- | :--- | :--- |
| **Trading Pair Symbol** | `TRUMP_USDT` | Base Asset: `TRUMP` / Quote Asset: `USDT` |
| **Candle Timeframe** | `1m` | Dynamic candle granularity evaluated by strategy indicators |
| **Strategy Evaluated** | `STOCH_RSI` | Stochastic RSI Momentum Scalper (Preset: FAST_SCALP ; Overbought/Oversold Reversal) |
| **Strategy Preset** | `FAST_SCALP` | Configured indicator preset profile |
| **Evaluation Date Range** | `2026-07-01` → `2026-07-24` | Historical evaluation window |
| **High-Fidelity Simulation** | `ENABLED (Tick Trades)` | Millisecond-level trade order matching & stop triggering |
| **Slippage Tolerance** | `0 ticks` (`0.000 USDT` per fill) | Adverse fill penalty applied to entry and exit orders |

### Strategy & Indicator Hyperparameters
| Hyperparameter | Value | Technical Context |
| :--- | :--- | :--- |
| **Active Strategy Engine** | `STOCH_RSI` | Quantitative model evaluated |
| **Active Strategy Preset** | `FAST_SCALP` | Selected preset configuration |
| **RSI Period** | `9` | Relative Strength Index calculation length |
| **Stoch Lookback Period** | `9` | Stochastic window over RSI |
| **%K Smoothing** | `3` | Fast stochastic line smoothing period |
| **%D Smoothing** | `3` | Slow signal line smoothing period |
| **Oversold Threshold (OS)** | `20.0` | Extreme oversold boundary (Bullish entry gate) |
| **Overbought Threshold (OB)** | `80.0` | Extreme overbought boundary (Bearish entry gate) |
| **Extreme Zone Filter** | `ENABLED` | Suppresses non-extreme neutral whipsaws |
| **Candle Close Confirmation** | `ENABLED` | Requires bar to close before emitting cross |
| **Directional Flow Mode** | `Autonomous Bi-Directional (LONG & SHORT)` | Order generation policy |

### Trade Optimization & Regime Filters
| Filter Dimension | Configuration | Operational Action & Trigger |
| :--- | :--- | :--- |
| **Trade Duration Monitoring** | `DISABLED` | Deep in-position monitoring at `60.0s` elapsed |
| **Time-Stop Protective Exit** | `DISABLED` | Action `CLOSE` triggered if open duration > `90.0s` |
| **ADX Trend Regime Filter** | `DISABLED` | Period: `14` / Threshold: `25.0` |
| **HTF Trend Baseline (200 EMA)** | `DISABLED` | Timeframe: `15m` / Period: `200` |
| **Hourly Session Filter** | `DISABLED` | Blacklisted UTC Hours: `None` |
| **Directional Bias Policy** | `BOTH` | Pre-trade signal directional allowance |

### Position Sizing, Leverage & Risk Management
| Risk Parameter | Value | Operational Details |
| :--- | :--- | :--- |
| **Sizing Mode** | `MULTIPLIER` | Mode: `CONTRACTS`, `MULTIPLIER`, or `MIN` |
| **Trade Volume / Quantity** | `2x minimum volume (2 contract(s))` | Quantity committed per trade signal |
| **Leverage Multiplier** | `75x` | Margin required = Position Notional / Leverage |
| **Starting Capital** | `0.07 USDT` | `₹6.61 INR` (`1 USDT = ₹94.45`) |
| **Take Profit Target** | `+3 ticks` (`+0.003 USDT`) | Guaranteed Min-Profit TP (`entry + N*pu`) |
| **Stop Loss Rule** | `-8 ticks away from entry (0.008 USDT)` | Stop loss evaluation logic |

### Exchange Contract Specifications & Fees
| Specification | Value | Notes |
| :--- | :--- | :--- |
| **Fee Schedule Mode** | `ZERO` | Live KCEX API, 0.0% zero-fee pair, or manual rate |
| **Maker Fee Rate** | `0.0000%` | Rate for passive limit orders |
| **Taker Fee Rate** | `0.0000%` | Rate for aggressive market / stop triggers |
| **Contract Size (cs)** | `0.1 TRUMP` | 1 contract = 0.1 underlying coin |
| **Price Unit (pu / tick)** | `0.001` | Minimum tick increment on order book |
| **Price Precision** | `3 decimal places` | Precision formatting for quotes and orders |
| **Min Volume** | `1.0 contract(s)` | Minimum permissible order size |
| **Max Leverage** | `75x` | Maximum allowed leverage on exchange |

---

## 📈 Trade Execution & Statistical Breakdown

| Metric | Value | Context / Benchmark |
| :--- | :--- | :--- |
| **Total Trades Executed** | `2031` | Total completed trade lifecycle events |
| **Winning Trades** | `1539` | `75.78%` of total trades |
| **Losing Trades** | `492` | `24.22%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0001 USDT` (`₹+0.01`) | Expected return per signal |
| **Average Winning Trade** | `+0.0006 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0016 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0006 USDT (+13.4% ROE)` | Trade #8 (LONG) |
| **Largest Losing Trade** | `-0.0016 USDT (-36.1% ROE)` | Trade #3 (LONG) |
| **Max Consecutive Wins** | `34` trades | Peak winning streak |
| **Max Consecutive Losses** | `6` trades | Peak losing streak |
| **Average Trade Duration** | `10m 43s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.5s` | Trade #164 |
| **Longest Trade In-Position** | `2h 36m 21s` | Trade #1399 |
| **Cumulative Time In Position** | `362h 53m 10s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1021` (50.3%) | `1010` (49.7%) | `2031` |
| **Wins / Losses** | `770 W / 251 L` | `769 W / 241 L` | `1539 W / 492 L` |
| **Win Rate** | **`75.42%`** | **`76.14%`** | **`75.78%`** |
| **Gross Profit** | `+0.4620 USDT` | `+0.4614 USDT` | `+0.9234 USDT` |
| **Gross Loss** | `-0.4016 USDT` | `-0.3856 USDT` | `-0.7872 USDT` |
| **Net Realized PnL** | **`+0.0604 USDT`** | **`+0.0758 USDT`** | **`+0.1362 USDT`** |
| **Net PnL (INR)** | `₹+5.70` | `₹+7.16` | `₹+12.86` |
| **Profit Factor** | `1.15` | `1.20` | `1.17` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1539` | `75.8%` | `+0.9234 USDT` | `₹+87.22` | `100.0%` | `8m 41s` |
| `STOP_LOSS_HIT` | `492` | `24.2%` | `-0.7872 USDT` | `₹-74.35` | `0.0%` | `17m 03s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:30:42 UTC | 1m 42s | `1.661` | `1.664` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.5%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 01:07:03 UTC | 30m 03s | `1.664` | `1.661` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.5%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 3 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:12:44 UTC | 2m 44s | `1.661` | `1.653` | $0.33 | $0.00 | $0.000000 | **-0.0016** | `-36.1%` | `STOP_LOSS_HIT` | $0.0696 |
| 4 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:04 UTC | 4.5s | `1.645` | `1.648` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.7%` | `MIN_PROFIT_TP_HIT` | $0.0702 |
| 5 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:24:25 UTC | 1m 25s | `1.658` | `1.655` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.6%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 6 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:38:45 UTC | 3m 45s | `1.658` | `1.666` | $0.33 | $0.00 | $0.000000 | **-0.0016** | `-36.2%` | `STOP_LOSS_HIT` | $0.0692 |
| 7 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:12 UTC | 2m 12s | `1.676` | `1.673` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.4%` | `MIN_PROFIT_TP_HIT` | $0.0698 |
| 8 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:55 UTC | 55.0s | `1.676` | `1.679` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.4%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 9 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:03:45 UTC | 4m 45s | `1.678` | `1.686` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.8%` | `STOP_LOSS_HIT` | $0.0688 |
| 10 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:10:04 UTC | 1m 04s | `1.684` | `1.687` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.4%` | `MIN_PROFIT_TP_HIT` | $0.0694 |
| 11 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:31:24 UTC | 13m 24s | `1.702` | `1.710` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.3%` | `STOP_LOSS_HIT` | $0.0678 |
| 12 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:29 UTC | 29.4s | `1.704` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 13 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:05 UTC | 3m 05s | `1.697` | `1.700` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.3%` | `MIN_PROFIT_TP_HIT` | $0.0690 |
| 14 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:39 UTC | 39.6s | `1.704` | `1.712` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.2%` | `STOP_LOSS_HIT` | $0.0674 |
| 15 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:32 UTC | 32.4s | `1.707` | `1.715` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.1%` | `STOP_LOSS_HIT` | $0.0658 |
| 16 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:08 UTC | 8.8s | `1.729` | `1.726` | $0.35 | $0.00 | $0.000000 | **+0.0006** | `+13.0%` | `MIN_PROFIT_TP_HIT` | $0.0664 |
| 17 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:30 UTC | 30.3s | `1.711` | `1.703` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.1%` | `STOP_LOSS_HIT` | $0.0648 |
| 18 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:24:02 UTC | 4m 02s | `1.704` | `1.696` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.2%` | `STOP_LOSS_HIT` | $0.0632 |
| 19 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:29:10 UTC | 1m 10s | `1.699` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0638 |
| 20 | `SHORT` | 2026-07-01 03:32:59 UTC | 2026-07-01 03:37:08 UTC | 4m 08s | `1.699` | `1.707` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.3%` | `STOP_LOSS_HIT` | $0.0622 |
| 21 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:52:16 UTC | 10m 16s | `1.706` | `1.714` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.2%` | `STOP_LOSS_HIT` | $0.0606 |
| 22 | `SHORT` | 2026-07-01 03:56:59 UTC | 2026-07-01 03:57:03 UTC | 3.6s | `1.712` | `1.709` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.1%` | `MIN_PROFIT_TP_HIT` | $0.0612 |
| 23 | `LONG` | 2026-07-01 04:02:59 UTC | 2026-07-01 04:05:04 UTC | 2m 04s | `1.705` | `1.708` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0618 |
| 24 | `LONG` | 2026-07-01 04:11:59 UTC | 2026-07-01 04:16:10 UTC | 4m 10s | `1.700` | `1.703` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0624 |
| 25 | `SHORT` | 2026-07-01 04:21:59 UTC | 2026-07-01 04:35:07 UTC | 13m 07s | `1.704` | `1.701` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0630 |
| ... | ... | *(1981 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2007 | `LONG` | 2026-07-23 17:04:59 UTC | 2026-07-23 17:40:40 UTC | 35m 40s | `1.621` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.0%` | `STOP_LOSS_HIT` | $0.2050 |
| 2008 | `SHORT` | 2026-07-23 17:47:59 UTC | 2026-07-23 17:53:23 UTC | 5m 23s | `1.611` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2056 |
| 2009 | `LONG` | 2026-07-23 18:02:59 UTC | 2026-07-23 18:05:47 UTC | 2m 47s | `1.599` | `1.591` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.5%` | `STOP_LOSS_HIT` | $0.2040 |
| 2010 | `SHORT` | 2026-07-23 18:12:59 UTC | 2026-07-23 18:17:24 UTC | 4m 24s | `1.594` | `1.591` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.1%` | `MIN_PROFIT_TP_HIT` | $0.2046 |
| 2011 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:37:12 UTC | 8m 12s | `1.610` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2052 |
| 2012 | `LONG` | 2026-07-23 18:40:59 UTC | 2026-07-23 18:52:55 UTC | 11m 55s | `1.608` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2058 |
| 2013 | `SHORT` | 2026-07-23 18:56:59 UTC | 2026-07-23 19:25:52 UTC | 28m 52s | `1.610` | `1.618` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.3%` | `STOP_LOSS_HIT` | $0.2042 |
| 2014 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:38:55 UTC | 9m 55s | `1.616` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.2048 |
| 2015 | `LONG` | 2026-07-23 19:40:59 UTC | 2026-07-23 19:59:06 UTC | 18m 06s | `1.613` | `1.616` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.2054 |
| 2016 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.2060 |
| 2017 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 21:04:40 UTC | 36m 40s | `1.623` | `1.626` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.2066 |
| 2018 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:08:20 UTC | 2m 20s | `1.622` | `1.619` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.2072 |
| 2019 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:31:59 UTC | 13m 59s | `1.617` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.1%` | `STOP_LOSS_HIT` | $0.2056 |
| 2020 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:44:51 UTC | 6m 51s | `1.603` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2062 |
| 2021 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 22:06:10 UTC | 20m 10s | `1.605` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.4%` | `STOP_LOSS_HIT` | $0.2046 |
| 2022 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:55 UTC | 5m 55s | `1.611` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2052 |
| 2023 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:49 UTC | 49.6s | `1.607` | `1.610` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2058 |
| 2024 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:40 UTC | 40.9s | `1.610` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2064 |
| 2025 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.2070 |
| 2026 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:38:25 UTC | 3m 25s | `1.611` | `1.603` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.2%` | `STOP_LOSS_HIT` | $0.2054 |
| 2027 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:41:44 UTC | 44.4s | `1.604` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2060 |
| 2028 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:40 UTC | 11m 40s | `1.607` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2066 |
| 2029 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:22:40 UTC | 13m 40s | `1.605` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2072 |
| 2030 | `SHORT` | 2026-07-23 23:24:59 UTC | 2026-07-23 23:47:35 UTC | 22m 35s | `1.607` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2078 |
| 2031 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:06:03 UTC | 11m 03s | `1.599` | `1.591` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.5%` | `STOP_LOSS_HIT` | $0.2062 |

> 💡 *Full granular dataset with all 2031 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
