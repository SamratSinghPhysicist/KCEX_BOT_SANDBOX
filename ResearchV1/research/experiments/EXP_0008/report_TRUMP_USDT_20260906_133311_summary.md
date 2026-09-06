# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:03:11 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.2568 USDT` | `₹24.25` | `+266.86%` |
| **Net Realized PnL** | **`+0.1868 USDT`** | **`₹+17.64`** | **`+266.86% Net ROI`** |
| **Gross Profit** | `+0.9260 USDT` | `₹87.46` | Total positive trade returns |
| **Gross Loss** | `-0.7392 USDT` | `₹69.82` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.25`** | — | Profitable |
| **Win / Loss Payoff** | `0.33` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0176 USDT` | `₹1.66` | **`-12.69%` Peak-to-Trough** |
| **Win Rate** | **`78.98%`** | — | `2315 Wins / 616 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `7.30` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `3.98` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `21.03` | — | Net ROI divided by Max Drawdown |

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
| **Take Profit Target** | `+2 ticks` (`+0.002 USDT`) | Guaranteed Min-Profit TP (`entry + N*pu`) |
| **Stop Loss Rule** | `-6 ticks away from entry (0.006 USDT)` | Stop loss evaluation logic |

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
| **Total Trades Executed** | `2931` | Total completed trade lifecycle events |
| **Winning Trades** | `2315` | `78.98%` of total trades |
| **Losing Trades** | `616` | `21.02%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0001 USDT` (`₹+0.01`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0012 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0012 USDT (-27.0% ROE)` | Trade #2 (SHORT) |
| **Max Consecutive Wins** | `26` trades | Peak winning streak |
| **Max Consecutive Losses** | `5` trades | Peak losing streak |
| **Average Trade Duration** | `5m 14s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #271 |
| **Longest Trade In-Position** | `1h 21m 43s` | Trade #2692 |
| **Cumulative Time In Position** | `256h 20m 58s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1450` (49.5%) | `1481` (50.5%) | `2931` |
| **Wins / Losses** | `1131 W / 319 L` | `1184 W / 297 L` | `2315 W / 616 L` |
| **Win Rate** | **`78.00%`** | **`79.95%`** | **`78.98%`** |
| **Gross Profit** | `+0.4524 USDT` | `+0.4736 USDT` | `+0.9260 USDT` |
| **Gross Loss** | `-0.3828 USDT` | `-0.3564 USDT` | `-0.7392 USDT` |
| **Net Realized PnL** | **`+0.0696 USDT`** | **`+0.1172 USDT`** | **`+0.1868 USDT`** |
| **Net PnL (INR)** | `₹+6.57` | `₹+11.07` | `₹+17.64` |
| **Profit Factor** | `1.18` | `1.33` | `1.25` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `2315` | `79.0%` | `+0.9260 USDT` | `₹+87.46` | `100.0%` | `3m 59s` |
| `STOP_LOSS_HIT` | `616` | `21.0%` | `-0.7392 USDT` | `₹-69.82` | `0.0%` | `9m 56s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:29:47 UTC | 47.6s | `1.661` | `1.663` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:52:46 UTC | 15m 46s | `1.664` | `1.670` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.0%` | `STOP_LOSS_HIT` | $0.0692 |
| 3 | `SHORT` | 2026-07-01 00:55:59 UTC | 2026-07-01 00:56:42 UTC | 42.7s | `1.669` | `1.667` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 4 | `LONG` | 2026-07-01 01:01:59 UTC | 2026-07-01 01:02:09 UTC | 9.1s | `1.667` | `1.669` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 5 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:12:29 UTC | 2m 29s | `1.661` | `1.655` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.1%` | `STOP_LOSS_HIT` | $0.0688 |
| 6 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:03 UTC | 3.2s | `1.645` | `1.647` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 7 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:23:12 UTC | 12.6s | `1.658` | `1.656` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 8 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:37:07 UTC | 2m 07s | `1.658` | `1.664` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.1%` | `STOP_LOSS_HIT` | $0.0684 |
| 9 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:09 UTC | 2m 09s | `1.676` | `1.674` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 10 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:10 UTC | 10.2s | `1.676` | `1.678` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 11 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:02:52 UTC | 3m 52s | `1.678` | `1.684` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.8%` | `STOP_LOSS_HIT` | $0.0680 |
| 12 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:06:09 UTC | 2m 09s | `1.685` | `1.679` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.7%` | `STOP_LOSS_HIT` | $0.0668 |
| 13 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:09:39 UTC | 39.7s | `1.684` | `1.686` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0672 |
| 14 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:22:05 UTC | 4m 05s | `1.702` | `1.708` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0660 |
| 15 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:13 UTC | 1m 13s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0664 |
| 16 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:05 UTC | 5.7s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 17 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:01 UTC | 3m 01s | `1.697` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0672 |
| 18 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:38 UTC | 38.4s | `1.704` | `1.710` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0660 |
| 19 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:24 UTC | 24.3s | `1.707` | `1.713` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0648 |
| 20 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:04 UTC | 4.8s | `1.729` | `1.727` | $0.35 | $0.00 | $0.000000 | **+0.0004** | `+8.7%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 21 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:27 UTC | 28.0s | `1.711` | `1.705` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.3%` | `STOP_LOSS_HIT` | $0.0640 |
| 22 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:23:46 UTC | 3m 46s | `1.704` | `1.698` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0628 |
| 23 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:29:01 UTC | 1m 01s | `1.699` | `1.701` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0632 |
| 24 | `SHORT` | 2026-07-01 03:32:59 UTC | 2026-07-01 03:34:17 UTC | 1m 17s | `1.699` | `1.697` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0636 |
| 25 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:47:31 UTC | 5m 31s | `1.706` | `1.712` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0624 |
| ... | ... | *(2881 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2907 | `SHORT` | 2026-07-23 18:17:59 UTC | 2026-07-23 18:18:03 UTC | 3.1s | `1.589` | `1.587` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2584 |
| 2908 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:30:28 UTC | 1m 28s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2588 |
| 2909 | `LONG` | 2026-07-23 18:35:59 UTC | 2026-07-23 18:45:08 UTC | 9m 08s | `1.610` | `1.604` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-28.0%` | `STOP_LOSS_HIT` | $0.2576 |
| 2910 | `LONG` | 2026-07-23 18:46:59 UTC | 2026-07-23 18:47:38 UTC | 38.7s | `1.606` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2580 |
| 2911 | `SHORT` | 2026-07-23 18:51:59 UTC | 2026-07-23 19:25:50 UTC | 33m 50s | `1.608` | `1.614` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-28.0%` | `STOP_LOSS_HIT` | $0.2568 |
| 2912 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:29:04 UTC | 4.2s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2572 |
| 2913 | `LONG` | 2026-07-23 19:40:59 UTC | 2026-07-23 19:51:13 UTC | 10m 13s | `1.613` | `1.607` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-27.9%` | `STOP_LOSS_HIT` | $0.2560 |
| 2914 | `LONG` | 2026-07-23 19:52:59 UTC | 2026-07-23 19:54:09 UTC | 1m 09s | `1.609` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2564 |
| 2915 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2568 |
| 2916 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 21:01:39 UTC | 33m 39s | `1.623` | `1.625` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2572 |
| 2917 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:07:45 UTC | 1m 45s | `1.622` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2576 |
| 2918 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:29:06 UTC | 11m 06s | `1.617` | `1.611` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-27.8%` | `STOP_LOSS_HIT` | $0.2564 |
| 2919 | `SHORT` | 2026-07-23 21:30:59 UTC | 2026-07-23 21:32:14 UTC | 1m 14s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2568 |
| 2920 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:38:30 UTC | 30.0s | `1.603` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2572 |
| 2921 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 22:05:02 UTC | 19m 02s | `1.605` | `1.611` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-28.0%` | `STOP_LOSS_HIT` | $0.2560 |
| 2922 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:17 UTC | 5m 17s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2564 |
| 2923 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:24 UTC | 24.5s | `1.607` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2568 |
| 2924 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:20 UTC | 20.1s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2572 |
| 2925 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2576 |
| 2926 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:37:43 UTC | 2m 43s | `1.611` | `1.605` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-27.9%` | `STOP_LOSS_HIT` | $0.2564 |
| 2927 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:41:36 UTC | 37.0s | `1.604` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2568 |
| 2928 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:35 UTC | 11m 35s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2572 |
| 2929 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:16:13 UTC | 7m 13s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2576 |
| 2930 | `SHORT` | 2026-07-23 23:19:59 UTC | 2026-07-23 23:47:35 UTC | 27m 35s | `1.606` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2580 |
| 2931 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:05:54 UTC | 10m 54s | `1.599` | `1.593` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-28.1%` | `STOP_LOSS_HIT` | $0.2568 |

> 💡 *Full granular dataset with all 2931 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
