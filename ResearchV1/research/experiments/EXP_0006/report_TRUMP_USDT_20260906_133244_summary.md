# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:02:45 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.2276 USDT` | `₹21.50` | `+225.14%` |
| **Net Realized PnL** | **`+0.1576 USDT`** | **`₹+14.89`** | **`+225.14% Net ROI`** |
| **Gross Profit** | `+0.9464 USDT` | `₹89.39` | Total positive trade returns |
| **Gross Loss** | `-0.7888 USDT` | `₹74.50` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.20`** | — | Profitable |
| **Win / Loss Payoff** | `0.50` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0116 USDT` | `₹1.10` | **`-8.08%` Peak-to-Trough** |
| **Win Rate** | **`70.58%`** | — | `2366 Wins / 986 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `6.76` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `4.65` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `27.86` | — | Net ROI divided by Max Drawdown |

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
| **Stop Loss Rule** | `-4 ticks away from entry (0.004 USDT)` | Stop loss evaluation logic |

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
| **Total Trades Executed** | `3352` | Total completed trade lifecycle events |
| **Winning Trades** | `2366` | `70.58%` of total trades |
| **Losing Trades** | `986` | `29.42%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0008 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0008 USDT (-18.0% ROE)` | Trade #2 (SHORT) |
| **Max Consecutive Wins** | `22` trades | Peak winning streak |
| **Max Consecutive Losses** | `6` trades | Peak losing streak |
| **Average Trade Duration** | `3m 39s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #302 |
| **Longest Trade In-Position** | `56m 41s` | Trade #1860 |
| **Cumulative Time In Position** | `204h 46m 21s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1640` (48.9%) | `1712` (51.1%) | `3352` |
| **Wins / Losses** | `1152 W / 488 L` | `1214 W / 498 L` | `2366 W / 986 L` |
| **Win Rate** | **`70.24%`** | **`70.91%`** | **`70.58%`** |
| **Gross Profit** | `+0.4608 USDT` | `+0.4856 USDT` | `+0.9464 USDT` |
| **Gross Loss** | `-0.3904 USDT` | `-0.3984 USDT` | `-0.7888 USDT` |
| **Net Realized PnL** | **`+0.0704 USDT`** | **`+0.0872 USDT`** | **`+0.1576 USDT`** |
| **Net PnL (INR)** | `₹+6.65` | `₹+8.24` | `₹+14.89` |
| **Profit Factor** | `1.18` | `1.22` | `1.20` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `2366` | `70.6%` | `+0.9464 USDT` | `₹+89.39` | `100.0%` | `2m 58s` |
| `STOP_LOSS_HIT` | `986` | `29.4%` | `-0.7888 USDT` | `₹-74.50` | `0.0%` | `5m 20s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:29:47 UTC | 47.6s | `1.661` | `1.663` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:52:00 UTC | 15m 00s | `1.664` | `1.668` | $0.33 | $0.00 | $0.000000 | **-0.0008** | `-18.0%` | `STOP_LOSS_HIT` | $0.0696 |
| 3 | `SHORT` | 2026-07-01 00:55:59 UTC | 2026-07-01 00:56:42 UTC | 42.7s | `1.669` | `1.667` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 4 | `LONG` | 2026-07-01 01:01:59 UTC | 2026-07-01 01:02:09 UTC | 9.1s | `1.667` | `1.669` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 5 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:10:57 UTC | 57.2s | `1.661` | `1.657` | $0.33 | $0.00 | $0.000000 | **-0.0008** | `-18.1%` | `STOP_LOSS_HIT` | $0.0696 |
| 6 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:03 UTC | 3.2s | `1.645` | `1.647` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 7 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:23:12 UTC | 12.6s | `1.658` | `1.656` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 8 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:35:43 UTC | 43.4s | `1.658` | `1.662` | $0.33 | $0.00 | $0.000000 | **-0.0008** | `-18.1%` | `STOP_LOSS_HIT` | $0.0696 |
| 9 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:09 UTC | 2m 09s | `1.676` | `1.674` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 10 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:10 UTC | 10.2s | `1.676` | `1.678` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 11 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:02:30 UTC | 3m 30s | `1.678` | `1.682` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.9%` | `STOP_LOSS_HIT` | $0.0696 |
| 12 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:04:58 UTC | 58.3s | `1.685` | `1.681` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.8%` | `STOP_LOSS_HIT` | $0.0688 |
| 13 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:09:39 UTC | 39.7s | `1.684` | `1.686` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 14 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:18:18 UTC | 18.2s | `1.702` | `1.706` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0684 |
| 15 | `LONG` | 2026-07-01 02:22:59 UTC | 2026-07-01 02:23:00 UTC | 0.9s | `1.709` | `1.705` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0676 |
| 16 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:13 UTC | 1m 13s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0680 |
| 17 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:05 UTC | 5.7s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 18 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:01 UTC | 3m 01s | `1.697` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 19 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:33 UTC | 33.3s | `1.704` | `1.708` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0680 |
| 20 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:07 UTC | 7.4s | `1.707` | `1.711` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0672 |
| 21 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:04 UTC | 4.8s | `1.729` | `1.727` | $0.35 | $0.00 | $0.000000 | **+0.0004** | `+8.7%` | `MIN_PROFIT_TP_HIT` | $0.0676 |
| 22 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:12 UTC | 12.1s | `1.711` | `1.707` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.5%` | `STOP_LOSS_HIT` | $0.0668 |
| 23 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:20:21 UTC | 21.5s | `1.704` | `1.700` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0660 |
| 24 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:29:01 UTC | 1m 01s | `1.699` | `1.701` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0664 |
| 25 | `SHORT` | 2026-07-01 03:32:59 UTC | 2026-07-01 03:34:17 UTC | 1m 17s | `1.699` | `1.697` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| ... | ... | *(3302 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 3328 | `LONG` | 2026-07-23 19:16:59 UTC | 2026-07-23 19:19:32 UTC | 2m 32s | `1.612` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.2276 |
| 3329 | `LONG` | 2026-07-23 19:22:59 UTC | 2026-07-23 19:23:49 UTC | 49.0s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2280 |
| 3330 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:29:04 UTC | 4.2s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2284 |
| 3331 | `LONG` | 2026-07-23 19:40:59 UTC | 2026-07-23 19:49:59 UTC | 8m 59s | `1.613` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.2276 |
| 3332 | `LONG` | 2026-07-23 19:52:59 UTC | 2026-07-23 19:54:09 UTC | 1m 09s | `1.609` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2280 |
| 3333 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2284 |
| 3334 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 20:40:29 UTC | 12m 29s | `1.623` | `1.619` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.5%` | `STOP_LOSS_HIT` | $0.2276 |
| 3335 | `LONG` | 2026-07-23 20:45:59 UTC | 2026-07-23 20:46:24 UTC | 24.0s | `1.618` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2280 |
| 3336 | `SHORT` | 2026-07-23 20:52:59 UTC | 2026-07-23 21:01:39 UTC | 8m 39s | `1.621` | `1.625` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.5%` | `STOP_LOSS_HIT` | $0.2272 |
| 3337 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:07:45 UTC | 1m 45s | `1.622` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2276 |
| 3338 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:18:08 UTC | 8.4s | `1.617` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.2268 |
| 3339 | `LONG` | 2026-07-23 21:22:59 UTC | 2026-07-23 21:30:11 UTC | 7m 11s | `1.614` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.2260 |
| 3340 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:38:30 UTC | 30.0s | `1.603` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2264 |
| 3341 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 21:55:50 UTC | 9m 50s | `1.605` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.7%` | `STOP_LOSS_HIT` | $0.2256 |
| 3342 | `SHORT` | 2026-07-23 22:00:59 UTC | 2026-07-23 22:02:05 UTC | 1m 05s | `1.609` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2260 |
| 3343 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:17 UTC | 5m 17s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2264 |
| 3344 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:24 UTC | 24.5s | `1.607` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2268 |
| 3345 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:20 UTC | 20.1s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2272 |
| 3346 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2276 |
| 3347 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:37:30 UTC | 2m 30s | `1.611` | `1.607` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.2268 |
| 3348 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:41:36 UTC | 37.0s | `1.604` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2272 |
| 3349 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:35 UTC | 11m 35s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2276 |
| 3350 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:16:13 UTC | 7m 13s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2280 |
| 3351 | `SHORT` | 2026-07-23 23:19:59 UTC | 2026-07-23 23:47:35 UTC | 27m 35s | `1.606` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2284 |
| 3352 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:03:59 UTC | 8m 59s | `1.599` | `1.595` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.8%` | `STOP_LOSS_HIT` | $0.2276 |

> 💡 *Full granular dataset with all 3352 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
