# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:08:43 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.2196 USDT` | `₹20.74` | `+213.71%` |
| **Net Realized PnL** | **`+0.1496 USDT`** | **`₹+14.13`** | **`+213.71% Net ROI`** |
| **Gross Profit** | `+0.8616 USDT` | `₹81.38` | Total positive trade returns |
| **Gross Loss** | `-0.7120 USDT` | `₹67.25` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.21`** | — | Profitable |
| **Win / Loss Payoff** | `0.40` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0156 USDT` | `₹1.47` | **`-15.43%` Peak-to-Trough** |
| **Win Rate** | **`75.16%`** | — | `2154 Wins / 712 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `6.36` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `3.85` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `13.85` | — | Net ROI divided by Max Drawdown |

---

## 🛠️ Complete Configuration & Settings Used

### Strategy & Market Setup
| Configuration Setting | Value | Operational Details |
| :--- | :--- | :--- |
| **Trading Pair Symbol** | `TRUMP_USDT` | Base Asset: `TRUMP` / Quote Asset: `USDT` |
| **Candle Timeframe** | `1m` | Dynamic candle granularity evaluated by strategy indicators |
| **Strategy Evaluated** | `STOCH_RSI` | Stochastic RSI Momentum Scalper (Preset: STANDARD ; Overbought/Oversold Reversal) |
| **Strategy Preset** | `STANDARD` | Configured indicator preset profile |
| **Evaluation Date Range** | `2026-07-01` → `2026-07-24` | Historical evaluation window |
| **High-Fidelity Simulation** | `ENABLED (Tick Trades)` | Millisecond-level trade order matching & stop triggering |
| **Slippage Tolerance** | `0 ticks` (`0.000 USDT` per fill) | Adverse fill penalty applied to entry and exit orders |

### Strategy & Indicator Hyperparameters
| Hyperparameter | Value | Technical Context |
| :--- | :--- | :--- |
| **Active Strategy Engine** | `STOCH_RSI` | Quantitative model evaluated |
| **Active Strategy Preset** | `STANDARD` | Selected preset configuration |
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
| **Stop Loss Rule** | `-5 ticks away from entry (0.005 USDT)` | Stop loss evaluation logic |

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
| **Total Trades Executed** | `2866` | Total completed trade lifecycle events |
| **Winning Trades** | `2154` | `75.16%` of total trades |
| **Losing Trades** | `712` | `24.84%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0001 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0010 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #2 (SHORT) |
| **Largest Losing Trade** | `-0.0010 USDT (-22.5% ROE)` | Trade #1 (SHORT) |
| **Max Consecutive Wins** | `24` trades | Peak winning streak |
| **Max Consecutive Losses** | `6` trades | Peak losing streak |
| **Average Trade Duration** | `4m 37s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #1744 |
| **Longest Trade In-Position** | `1h 04m 06s` | Trade #1527 |
| **Cumulative Time In Position** | `220h 35m 09s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1410` (49.2%) | `1456` (50.8%) | `2866` |
| **Wins / Losses** | `1045 W / 365 L` | `1109 W / 347 L` | `2154 W / 712 L` |
| **Win Rate** | **`74.11%`** | **`76.17%`** | **`75.16%`** |
| **Gross Profit** | `+0.4180 USDT` | `+0.4436 USDT` | `+0.8616 USDT` |
| **Gross Loss** | `-0.3650 USDT` | `-0.3470 USDT` | `-0.7120 USDT` |
| **Net Realized PnL** | **`+0.0530 USDT`** | **`+0.0966 USDT`** | **`+0.1496 USDT`** |
| **Net PnL (INR)** | `₹+5.01` | `₹+9.12` | `₹+14.13` |
| **Profit Factor** | `1.15` | `1.28` | `1.21` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `STOP_LOSS_HIT` | `712` | `24.8%` | `-0.7120 USDT` | `₹-67.25` | `0.0%` | `7m 22s` |
| `MIN_PROFIT_TP_HIT` | `2154` | `75.2%` | `+0.8616 USDT` | `₹+81.38` | `100.0%` | `3m 42s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:52:44 UTC | 15m 44s | `1.664` | `1.669` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.5%` | `STOP_LOSS_HIT` | $0.0690 |
| 2 | `SHORT` | 2026-07-01 00:56:59 UTC | 2026-07-01 00:58:49 UTC | 1m 49s | `1.667` | `1.665` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0694 |
| 3 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:11:30 UTC | 1m 30s | `1.661` | `1.656` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.6%` | `STOP_LOSS_HIT` | $0.0684 |
| 4 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:03 UTC | 3.2s | `1.645` | `1.647` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 5 | `SHORT` | 2026-07-01 01:24:59 UTC | 2026-07-01 01:29:22 UTC | 4m 22s | `1.653` | `1.658` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.7%` | `STOP_LOSS_HIT` | $0.0678 |
| 6 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:36:14 UTC | 1m 14s | `1.658` | `1.663` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.6%` | `STOP_LOSS_HIT` | $0.0668 |
| 7 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:09 UTC | 2m 09s | `1.676` | `1.674` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0672 |
| 8 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:05:51 UTC | 1m 51s | `1.685` | `1.680` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.3%` | `STOP_LOSS_HIT` | $0.0662 |
| 9 | `LONG` | 2026-07-01 02:09:59 UTC | 2026-07-01 02:10:04 UTC | 4.2s | `1.685` | `1.687` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0666 |
| 10 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:22:04 UTC | 4m 04s | `1.702` | `1.707` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0656 |
| 11 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:13 UTC | 1m 13s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0660 |
| 12 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:05 UTC | 5.7s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0664 |
| 13 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:01 UTC | 3m 01s | `1.697` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 14 | `LONG` | 2026-07-01 02:50:59 UTC | 2026-07-01 02:52:26 UTC | 1m 26s | `1.699` | `1.694` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.1%` | `STOP_LOSS_HIT` | $0.0658 |
| 15 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:07 UTC | 7.4s | `1.707` | `1.712` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0648 |
| 16 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:04 UTC | 4.8s | `1.729` | `1.727` | $0.35 | $0.00 | $0.000000 | **+0.0004** | `+8.7%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 17 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:23:46 UTC | 3m 46s | `1.704` | `1.699` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0642 |
| 18 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:29:01 UTC | 1m 01s | `1.699` | `1.701` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0646 |
| 19 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:47:01 UTC | 5m 01s | `1.706` | `1.711` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0636 |
| 20 | `SHORT` | 2026-07-01 03:48:59 UTC | 2026-07-01 03:50:57 UTC | 1m 57s | `1.706` | `1.711` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0626 |
| 21 | `LONG` | 2026-07-01 04:02:59 UTC | 2026-07-01 04:04:04 UTC | 1m 04s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0630 |
| 22 | `LONG` | 2026-07-01 04:11:59 UTC | 2026-07-01 04:16:02 UTC | 4m 02s | `1.700` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0634 |
| 23 | `SHORT` | 2026-07-01 04:21:59 UTC | 2026-07-01 04:23:55 UTC | 1m 55s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0638 |
| 24 | `SHORT` | 2026-07-01 04:30:59 UTC | 2026-07-01 04:31:23 UTC | 23.4s | `1.705` | `1.710` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0628 |
| 25 | `SHORT` | 2026-07-01 04:34:59 UTC | 2026-07-01 04:35:07 UTC | 7.3s | `1.703` | `1.701` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0632 |
| ... | ... | *(2816 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2842 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:30:28 UTC | 1m 28s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2198 |
| 2843 | `LONG` | 2026-07-23 18:46:59 UTC | 2026-07-23 18:47:38 UTC | 38.7s | `1.606` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2202 |
| 2844 | `SHORT` | 2026-07-23 18:56:59 UTC | 2026-07-23 18:58:39 UTC | 1m 39s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2206 |
| 2845 | `LONG` | 2026-07-23 19:10:59 UTC | 2026-07-23 19:11:08 UTC | 8.6s | `1.609` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2210 |
| 2846 | `LONG` | 2026-07-23 19:16:59 UTC | 2026-07-23 19:25:50 UTC | 8m 50s | `1.612` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2214 |
| 2847 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:29:04 UTC | 4.2s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2218 |
| 2848 | `LONG` | 2026-07-23 19:40:59 UTC | 2026-07-23 19:50:07 UTC | 9m 07s | `1.613` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.2208 |
| 2849 | `LONG` | 2026-07-23 19:52:59 UTC | 2026-07-23 19:54:09 UTC | 1m 09s | `1.609` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2212 |
| 2850 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2216 |
| 2851 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 20:40:43 UTC | 12m 43s | `1.623` | `1.618` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.2206 |
| 2852 | `SHORT` | 2026-07-23 20:57:59 UTC | 2026-07-23 21:07:01 UTC | 9m 01s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2210 |
| 2853 | `LONG` | 2026-07-23 21:12:59 UTC | 2026-07-23 21:13:00 UTC | 0.2s | `1.619` | `1.614` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.2200 |
| 2854 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:18:27 UTC | 27.3s | `1.617` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.2190 |
| 2855 | `LONG` | 2026-07-23 21:22:59 UTC | 2026-07-23 21:31:59 UTC | 8m 59s | `1.614` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.2180 |
| 2856 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:38:30 UTC | 30.0s | `1.603` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2184 |
| 2857 | `SHORT` | 2026-07-23 21:48:59 UTC | 2026-07-23 21:56:25 UTC | 7m 25s | `1.605` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.4%` | `STOP_LOSS_HIT` | $0.2174 |
| 2858 | `SHORT` | 2026-07-23 22:00:59 UTC | 2026-07-23 22:02:05 UTC | 1m 05s | `1.609` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2178 |
| 2859 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:17 UTC | 5m 17s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2182 |
| 2860 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:20 UTC | 20.1s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2186 |
| 2861 | `SHORT` | 2026-07-23 22:28:59 UTC | 2026-07-23 22:29:23 UTC | 23.5s | `1.615` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2190 |
| 2862 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:41:36 UTC | 37.0s | `1.604` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2194 |
| 2863 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:35 UTC | 11m 35s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2198 |
| 2864 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:16:13 UTC | 7m 13s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2202 |
| 2865 | `SHORT` | 2026-07-23 23:19:59 UTC | 2026-07-23 23:47:35 UTC | 27m 35s | `1.606` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2206 |
| 2866 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:05:13 UTC | 10m 13s | `1.599` | `1.594` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.5%` | `STOP_LOSS_HIT` | $0.2196 |

> 💡 *Full granular dataset with all 2866 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
