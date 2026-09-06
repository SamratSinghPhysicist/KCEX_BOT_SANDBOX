# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:12:53 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.2534 USDT` | `₹23.93` | `+262.00%` |
| **Net Realized PnL** | **`+0.1834 USDT`** | **`₹+17.32`** | **`+262.00% Net ROI`** |
| **Gross Profit** | `+0.8644 USDT` | `₹81.64` | Total positive trade returns |
| **Gross Loss** | `-0.6810 USDT` | `₹64.32` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.27`** | — | Profitable |
| **Win / Loss Payoff** | `0.40` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0178 USDT` | `₹1.68` | **`-8.24%` Peak-to-Trough** |
| **Win Rate** | **`76.04%`** | — | `2161 Wins / 681 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `8.11` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `4.86` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `31.80` | — | Net ROI divided by Max Drawdown |

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
| **ADX Trend Regime Filter** | `ENABLED` | Period: `14` / Threshold: `15.0` |
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
| **Total Trades Executed** | `2842` | Total completed trade lifecycle events |
| **Winning Trades** | `2161` | `76.04%` of total trades |
| **Losing Trades** | `681` | `23.96%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0001 USDT` (`₹+0.01`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0010 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0010 USDT (-22.5% ROE)` | Trade #2 (SHORT) |
| **Max Consecutive Wins** | `22` trades | Peak winning streak |
| **Max Consecutive Losses** | `7` trades | Peak losing streak |
| **Average Trade Duration** | `4m 37s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #252 |
| **Longest Trade In-Position** | `1h 15m 46s` | Trade #1388 |
| **Cumulative Time In Position** | `219h 09m 45s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1388` (48.8%) | `1454` (51.2%) | `2842` |
| **Wins / Losses** | `1042 W / 346 L` | `1119 W / 335 L` | `2161 W / 681 L` |
| **Win Rate** | **`75.07%`** | **`76.96%`** | **`76.04%`** |
| **Gross Profit** | `+0.4168 USDT` | `+0.4476 USDT` | `+0.8644 USDT` |
| **Gross Loss** | `-0.3460 USDT` | `-0.3350 USDT` | `-0.6810 USDT` |
| **Net Realized PnL** | **`+0.0708 USDT`** | **`+0.1126 USDT`** | **`+0.1834 USDT`** |
| **Net PnL (INR)** | `₹+6.69` | `₹+10.64` | `₹+17.32` |
| **Profit Factor** | `1.20` | `1.34` | `1.27` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `2161` | `76.0%` | `+0.8644 USDT` | `₹+81.64` | `100.0%` | `3m 44s` |
| `STOP_LOSS_HIT` | `681` | `24.0%` | `-0.6810 USDT` | `₹-64.32` | `0.0%` | `7m 26s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:29:47 UTC | 47.6s | `1.661` | `1.663` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:52:44 UTC | 15m 44s | `1.664` | `1.669` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.5%` | `STOP_LOSS_HIT` | $0.0694 |
| 3 | `SHORT` | 2026-07-01 00:55:59 UTC | 2026-07-01 00:56:42 UTC | 42.7s | `1.669` | `1.667` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0698 |
| 4 | `LONG` | 2026-07-01 01:01:59 UTC | 2026-07-01 01:02:09 UTC | 9.1s | `1.667` | `1.669` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0702 |
| 5 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:11:30 UTC | 1m 30s | `1.661` | `1.656` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.6%` | `STOP_LOSS_HIT` | $0.0692 |
| 6 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:03 UTC | 3.2s | `1.645` | `1.647` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 7 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:23:12 UTC | 12.6s | `1.658` | `1.656` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 8 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:36:14 UTC | 1m 14s | `1.658` | `1.663` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.6%` | `STOP_LOSS_HIT` | $0.0690 |
| 9 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:09 UTC | 2m 09s | `1.676` | `1.674` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0694 |
| 10 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:10 UTC | 10.2s | `1.676` | `1.678` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0698 |
| 11 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:02:36 UTC | 3m 36s | `1.678` | `1.683` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.3%` | `STOP_LOSS_HIT` | $0.0688 |
| 12 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:05:51 UTC | 1m 51s | `1.685` | `1.680` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.3%` | `STOP_LOSS_HIT` | $0.0678 |
| 13 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:09:39 UTC | 39.7s | `1.684` | `1.686` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0682 |
| 14 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:22:04 UTC | 4m 04s | `1.702` | `1.707` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0672 |
| 15 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:13 UTC | 1m 13s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0676 |
| 16 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:05 UTC | 5.7s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0680 |
| 17 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:01 UTC | 3m 01s | `1.697` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 18 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:34 UTC | 34.2s | `1.704` | `1.709` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0674 |
| 19 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:07 UTC | 7.4s | `1.707` | `1.712` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0664 |
| 20 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:04 UTC | 4.8s | `1.729` | `1.727` | $0.35 | $0.00 | $0.000000 | **+0.0004** | `+8.7%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 21 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:12 UTC | 12.1s | `1.711` | `1.706` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-21.9%` | `STOP_LOSS_HIT` | $0.0658 |
| 22 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:23:46 UTC | 3m 46s | `1.704` | `1.699` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0648 |
| 23 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:29:01 UTC | 1m 01s | `1.699` | `1.701` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 24 | `SHORT` | 2026-07-01 03:32:59 UTC | 2026-07-01 03:34:17 UTC | 1m 17s | `1.699` | `1.697` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0656 |
| 25 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:47:01 UTC | 5m 01s | `1.706` | `1.711` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0646 |
| ... | ... | *(2792 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2818 | `LONG` | 2026-07-23 18:46:59 UTC | 2026-07-23 18:47:38 UTC | 38.7s | `1.606` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2564 |
| 2819 | `SHORT` | 2026-07-23 18:51:59 UTC | 2026-07-23 19:12:14 UTC | 20m 14s | `1.608` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.2554 |
| 2820 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:29:04 UTC | 4.2s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2558 |
| 2821 | `LONG` | 2026-07-23 19:47:59 UTC | 2026-07-23 19:50:07 UTC | 2m 07s | `1.613` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.2548 |
| 2822 | `LONG` | 2026-07-23 19:52:59 UTC | 2026-07-23 19:54:09 UTC | 1m 09s | `1.609` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2552 |
| 2823 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2556 |
| 2824 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 20:40:43 UTC | 12m 43s | `1.623` | `1.618` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.2546 |
| 2825 | `LONG` | 2026-07-23 20:45:59 UTC | 2026-07-23 20:46:24 UTC | 24.0s | `1.618` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2550 |
| 2826 | `SHORT` | 2026-07-23 20:52:59 UTC | 2026-07-23 21:04:40 UTC | 11m 40s | `1.621` | `1.626` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.2540 |
| 2827 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:07:45 UTC | 1m 45s | `1.622` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2544 |
| 2828 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:18:27 UTC | 27.3s | `1.617` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.2534 |
| 2829 | `LONG` | 2026-07-23 21:22:59 UTC | 2026-07-23 21:31:59 UTC | 8m 59s | `1.614` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.2524 |
| 2830 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:38:30 UTC | 30.0s | `1.603` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2528 |
| 2831 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 21:56:25 UTC | 10m 25s | `1.605` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.4%` | `STOP_LOSS_HIT` | $0.2518 |
| 2832 | `SHORT` | 2026-07-23 22:00:59 UTC | 2026-07-23 22:02:05 UTC | 1m 05s | `1.609` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2522 |
| 2833 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:17 UTC | 5m 17s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2526 |
| 2834 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:24 UTC | 24.5s | `1.607` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2530 |
| 2835 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:20 UTC | 20.1s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2534 |
| 2836 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2538 |
| 2837 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:37:30 UTC | 2m 30s | `1.611` | `1.606` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.2528 |
| 2838 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:41:36 UTC | 37.0s | `1.604` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2532 |
| 2839 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:35 UTC | 11m 35s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2536 |
| 2840 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:16:13 UTC | 7m 13s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2540 |
| 2841 | `SHORT` | 2026-07-23 23:19:59 UTC | 2026-07-23 23:47:35 UTC | 27m 35s | `1.606` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2544 |
| 2842 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:05:13 UTC | 10m 13s | `1.599` | `1.594` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.5%` | `STOP_LOSS_HIT` | $0.2534 |

> 💡 *Full granular dataset with all 2842 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
