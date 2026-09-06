# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:09:14 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.2200 USDT` | `₹20.78` | `+214.29%` |
| **Net Realized PnL** | **`+0.1500 USDT`** | **`₹+14.17`** | **`+214.29% Net ROI`** |
| **Gross Profit** | `+0.9068 USDT` | `₹85.65` | Total positive trade returns |
| **Gross Loss** | `-0.7568 USDT` | `₹71.48` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.20`** | — | Profitable |
| **Win / Loss Payoff** | `0.50` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0112 USDT` | `₹1.06` | **`-14.29%` Peak-to-Trough** |
| **Win Rate** | **`70.56%`** | — | `2267 Wins / 946 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `6.36` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `4.35` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `15.00` | — | Net ROI divided by Max Drawdown |

---

## 🛠️ Complete Configuration & Settings Used

### Strategy & Market Setup
| Configuration Setting | Value | Operational Details |
| :--- | :--- | :--- |
| **Trading Pair Symbol** | `TRUMP_USDT` | Base Asset: `TRUMP` / Quote Asset: `USDT` |
| **Candle Timeframe** | `1m` | Dynamic candle granularity evaluated by strategy indicators |
| **Strategy Evaluated** | `STOCH_RSI` | Stochastic RSI Momentum Scalper (Preset: MICRO_BURST ; Overbought/Oversold Reversal) |
| **Strategy Preset** | `MICRO_BURST` | Configured indicator preset profile |
| **Evaluation Date Range** | `2026-07-01` → `2026-07-24` | Historical evaluation window |
| **High-Fidelity Simulation** | `ENABLED (Tick Trades)` | Millisecond-level trade order matching & stop triggering |
| **Slippage Tolerance** | `0 ticks` (`0.000 USDT` per fill) | Adverse fill penalty applied to entry and exit orders |

### Strategy & Indicator Hyperparameters
| Hyperparameter | Value | Technical Context |
| :--- | :--- | :--- |
| **Active Strategy Engine** | `STOCH_RSI` | Quantitative model evaluated |
| **Active Strategy Preset** | `MICRO_BURST` | Selected preset configuration |
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
| **Total Trades Executed** | `3213` | Total completed trade lifecycle events |
| **Winning Trades** | `2267` | `70.56%` of total trades |
| **Losing Trades** | `946` | `29.44%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0008 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (SHORT) |
| **Largest Losing Trade** | `-0.0008 USDT (-18.0% ROE)` | Trade #3 (SHORT) |
| **Max Consecutive Wins** | `20` trades | Peak winning streak |
| **Max Consecutive Losses** | `6` trades | Peak losing streak |
| **Average Trade Duration** | `3m 34s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #2523 |
| **Longest Trade In-Position** | `1h 05m 41s` | Trade #1777 |
| **Cumulative Time In Position** | `191h 35m 11s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1577` (49.1%) | `1636` (50.9%) | `3213` |
| **Wins / Losses** | `1102 W / 475 L` | `1165 W / 471 L` | `2267 W / 946 L` |
| **Win Rate** | **`69.88%`** | **`71.21%`** | **`70.56%`** |
| **Gross Profit** | `+0.4408 USDT` | `+0.4660 USDT` | `+0.9068 USDT` |
| **Gross Loss** | `-0.3800 USDT` | `-0.3768 USDT` | `-0.7568 USDT` |
| **Net Realized PnL** | **`+0.0608 USDT`** | **`+0.0892 USDT`** | **`+0.1500 USDT`** |
| **Net PnL (INR)** | `₹+5.74` | `₹+8.42` | `₹+14.17` |
| **Profit Factor** | `1.16` | `1.24` | `1.20` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `2267` | `70.6%` | `+0.9068 USDT` | `₹+85.65` | `100.0%` | `2m 53s` |
| `STOP_LOSS_HIT` | `946` | `29.4%` | `-0.7568 USDT` | `₹-71.48` | `0.0%` | `5m 13s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `SHORT` | 2026-07-01 00:22:59 UTC | 2026-07-01 00:23:55 UTC | 55.2s | `1.661` | `1.659` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:29:47 UTC | 47.6s | `1.661` | `1.663` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 3 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:52:00 UTC | 15m 00s | `1.664` | `1.668` | $0.33 | $0.00 | $0.000000 | **-0.0008** | `-18.0%` | `STOP_LOSS_HIT` | $0.0700 |
| 4 | `SHORT` | 2026-07-01 00:55:59 UTC | 2026-07-01 00:56:42 UTC | 42.7s | `1.669` | `1.667` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 5 | `LONG` | 2026-07-01 01:01:59 UTC | 2026-07-01 01:02:09 UTC | 9.1s | `1.667` | `1.669` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 6 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:10:57 UTC | 57.2s | `1.661` | `1.657` | $0.33 | $0.00 | $0.000000 | **-0.0008** | `-18.1%` | `STOP_LOSS_HIT` | $0.0700 |
| 7 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:03 UTC | 3.2s | `1.645` | `1.647` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 8 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:23:12 UTC | 12.6s | `1.658` | `1.656` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 9 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:35:43 UTC | 43.4s | `1.658` | `1.662` | $0.33 | $0.00 | $0.000000 | **-0.0008** | `-18.1%` | `STOP_LOSS_HIT` | $0.0700 |
| 10 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:09 UTC | 2m 09s | `1.676` | `1.674` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 11 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:10 UTC | 10.2s | `1.676` | `1.678` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 12 | `SHORT` | 2026-07-01 01:57:59 UTC | 2026-07-01 01:58:04 UTC | 4.4s | `1.682` | `1.680` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 13 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:18:18 UTC | 18.2s | `1.702` | `1.706` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0704 |
| 14 | `LONG` | 2026-07-01 02:22:59 UTC | 2026-07-01 02:23:00 UTC | 0.9s | `1.709` | `1.705` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0696 |
| 15 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:13 UTC | 1m 13s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 16 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:05 UTC | 5.7s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 17 | `SHORT` | 2026-07-01 02:47:59 UTC | 2026-07-01 02:50:20 UTC | 2m 20s | `1.697` | `1.701` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.7%` | `STOP_LOSS_HIT` | $0.0696 |
| 18 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:07 UTC | 7.4s | `1.707` | `1.711` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0688 |
| 19 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:04 UTC | 4.8s | `1.729` | `1.727` | $0.35 | $0.00 | $0.000000 | **+0.0004** | `+8.7%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 20 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:12 UTC | 12.1s | `1.711` | `1.707` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.5%` | `STOP_LOSS_HIT` | $0.0684 |
| 21 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:20:21 UTC | 21.5s | `1.704` | `1.700` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0676 |
| 22 | `SHORT` | 2026-07-01 03:31:59 UTC | 2026-07-01 03:32:27 UTC | 27.8s | `1.698` | `1.696` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0680 |
| 23 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:46:48 UTC | 4m 48s | `1.706` | `1.710` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0672 |
| 24 | `LONG` | 2026-07-01 03:51:59 UTC | 2026-07-01 03:52:16 UTC | 16.2s | `1.711` | `1.713` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0676 |
| 25 | `SHORT` | 2026-07-01 03:56:59 UTC | 2026-07-01 03:57:03 UTC | 3.5s | `1.712` | `1.710` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0680 |
| ... | ... | *(3163 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 3189 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:30:28 UTC | 1m 28s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2260 |
| 3190 | `LONG` | 2026-07-23 18:34:59 UTC | 2026-07-23 18:41:11 UTC | 6m 11s | `1.610` | `1.606` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.2252 |
| 3191 | `LONG` | 2026-07-23 18:46:59 UTC | 2026-07-23 18:47:38 UTC | 38.7s | `1.606` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2256 |
| 3192 | `SHORT` | 2026-07-23 18:51:59 UTC | 2026-07-23 19:02:40 UTC | 10m 40s | `1.608` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.7%` | `STOP_LOSS_HIT` | $0.2248 |
| 3193 | `SHORT` | 2026-07-23 19:19:59 UTC | 2026-07-23 19:25:14 UTC | 5m 14s | `1.609` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.2240 |
| 3194 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:29:04 UTC | 4.2s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2244 |
| 3195 | `LONG` | 2026-07-23 19:33:59 UTC | 2026-07-23 19:41:22 UTC | 7m 22s | `1.616` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.2236 |
| 3196 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2240 |
| 3197 | `SHORT` | 2026-07-23 20:33:59 UTC | 2026-07-23 20:40:12 UTC | 6m 12s | `1.622` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2244 |
| 3198 | `LONG` | 2026-07-23 20:45:59 UTC | 2026-07-23 20:46:24 UTC | 24.0s | `1.618` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2248 |
| 3199 | `SHORT` | 2026-07-23 20:52:59 UTC | 2026-07-23 21:01:39 UTC | 8m 39s | `1.621` | `1.625` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.5%` | `STOP_LOSS_HIT` | $0.2240 |
| 3200 | `LONG` | 2026-07-23 21:13:59 UTC | 2026-07-23 21:18:27 UTC | 4m 27s | `1.616` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.2232 |
| 3201 | `LONG` | 2026-07-23 21:22:59 UTC | 2026-07-23 21:30:11 UTC | 7m 11s | `1.614` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.2224 |
| 3202 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:38:30 UTC | 30.0s | `1.603` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2228 |
| 3203 | `SHORT` | 2026-07-23 21:48:59 UTC | 2026-07-23 21:55:50 UTC | 6m 50s | `1.605` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.7%` | `STOP_LOSS_HIT` | $0.2220 |
| 3204 | `SHORT` | 2026-07-23 22:00:59 UTC | 2026-07-23 22:02:05 UTC | 1m 05s | `1.609` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2224 |
| 3205 | `LONG` | 2026-07-23 22:15:59 UTC | 2026-07-23 22:17:55 UTC | 1m 55s | `1.612` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.2216 |
| 3206 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:20 UTC | 20.1s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2220 |
| 3207 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2224 |
| 3208 | `LONG` | 2026-07-23 22:33:59 UTC | 2026-07-23 22:37:30 UTC | 3m 30s | `1.611` | `1.607` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.2216 |
| 3209 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:41:36 UTC | 37.0s | `1.604` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2220 |
| 3210 | `LONG` | 2026-07-23 22:54:59 UTC | 2026-07-23 23:01:40 UTC | 6m 40s | `1.608` | `1.604` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.7%` | `STOP_LOSS_HIT` | $0.2212 |
| 3211 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:16:13 UTC | 7m 13s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2216 |
| 3212 | `SHORT` | 2026-07-23 23:18:59 UTC | 2026-07-23 23:25:35 UTC | 6m 35s | `1.605` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.7%` | `STOP_LOSS_HIT` | $0.2208 |
| 3213 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:03:59 UTC | 8m 59s | `1.599` | `1.595` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.8%` | `STOP_LOSS_HIT` | $0.2200 |

> 💡 *Full granular dataset with all 3213 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
