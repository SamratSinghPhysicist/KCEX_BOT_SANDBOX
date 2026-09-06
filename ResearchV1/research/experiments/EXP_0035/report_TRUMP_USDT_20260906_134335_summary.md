# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:13:35 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.1996 USDT` | `₹18.85` | `+185.14%` |
| **Net Realized PnL** | **`+0.1296 USDT`** | **`₹+12.24`** | **`+185.14% Net ROI`** |
| **Gross Profit** | `+0.6776 USDT` | `₹64.00` | Total positive trade returns |
| **Gross Loss** | `-0.5480 USDT` | `₹51.76` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.24`** | — | Profitable |
| **Win / Loss Payoff** | `0.40` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0108 USDT` | `₹1.02` | **`-7.42%` Peak-to-Trough** |
| **Win Rate** | **`75.56%`** | — | `1694 Wins / 548 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `7.63` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `4.61` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `24.96` | — | Net ROI divided by Max Drawdown |

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
| **ADX Trend Regime Filter** | `ENABLED` | Period: `14` / Threshold: `20.0` |
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
| **Total Trades Executed** | `2242` | Total completed trade lifecycle events |
| **Winning Trades** | `1694` | `75.56%` of total trades |
| **Losing Trades** | `548` | `24.44%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0001 USDT` (`₹+0.01`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0010 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0010 USDT (-22.5% ROE)` | Trade #2 (SHORT) |
| **Max Consecutive Wins** | `25` trades | Peak winning streak |
| **Max Consecutive Losses** | `5` trades | Peak losing streak |
| **Average Trade Duration** | `4m 35s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #189 |
| **Longest Trade In-Position** | `1h 17m 06s` | Trade #1101 |
| **Cumulative Time In Position** | `171h 24m 11s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1107` (49.4%) | `1135` (50.6%) | `2242` |
| **Wins / Losses** | `829 W / 278 L` | `865 W / 270 L` | `1694 W / 548 L` |
| **Win Rate** | **`74.89%`** | **`76.21%`** | **`75.56%`** |
| **Gross Profit** | `+0.3316 USDT` | `+0.3460 USDT` | `+0.6776 USDT` |
| **Gross Loss** | `-0.2780 USDT` | `-0.2700 USDT` | `-0.5480 USDT` |
| **Net Realized PnL** | **`+0.0536 USDT`** | **`+0.0760 USDT`** | **`+0.1296 USDT`** |
| **Net PnL (INR)** | `₹+5.06` | `₹+7.18` | `₹+12.24` |
| **Profit Factor** | `1.19` | `1.28` | `1.24` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1694` | `75.6%` | `+0.6776 USDT` | `₹+64.00` | `100.0%` | `3m 38s` |
| `STOP_LOSS_HIT` | `548` | `24.4%` | `-0.5480 USDT` | `₹-51.76` | `0.0%` | `7m 29s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:29:47 UTC | 47.6s | `1.661` | `1.663` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:52:44 UTC | 15m 44s | `1.664` | `1.669` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.5%` | `STOP_LOSS_HIT` | $0.0694 |
| 3 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:11:30 UTC | 1m 30s | `1.661` | `1.656` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.6%` | `STOP_LOSS_HIT` | $0.0684 |
| 4 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:03 UTC | 3.2s | `1.645` | `1.647` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 5 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:23:12 UTC | 12.6s | `1.658` | `1.656` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 6 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:09 UTC | 2m 09s | `1.676` | `1.674` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 7 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:10 UTC | 10.2s | `1.676` | `1.678` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 8 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:02:36 UTC | 3m 36s | `1.678` | `1.683` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.3%` | `STOP_LOSS_HIT` | $0.0690 |
| 9 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:05:51 UTC | 1m 51s | `1.685` | `1.680` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.3%` | `STOP_LOSS_HIT` | $0.0680 |
| 10 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:09:39 UTC | 39.7s | `1.684` | `1.686` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 11 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:22:04 UTC | 4m 04s | `1.702` | `1.707` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0674 |
| 12 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:13 UTC | 1m 13s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0678 |
| 13 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:05 UTC | 5.7s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0682 |
| 14 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:01 UTC | 3m 01s | `1.697` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0686 |
| 15 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:07 UTC | 7.4s | `1.707` | `1.712` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0676 |
| 16 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:04 UTC | 4.8s | `1.729` | `1.727` | $0.35 | $0.00 | $0.000000 | **+0.0004** | `+8.7%` | `MIN_PROFIT_TP_HIT` | $0.0680 |
| 17 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:12 UTC | 12.1s | `1.711` | `1.706` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-21.9%` | `STOP_LOSS_HIT` | $0.0670 |
| 18 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:23:46 UTC | 3m 46s | `1.704` | `1.699` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0660 |
| 19 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:29:01 UTC | 1m 01s | `1.699` | `1.701` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0664 |
| 20 | `SHORT` | 2026-07-01 03:32:59 UTC | 2026-07-01 03:34:17 UTC | 1m 17s | `1.699` | `1.697` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 21 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:47:01 UTC | 5m 01s | `1.706` | `1.711` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0658 |
| 22 | `LONG` | 2026-07-01 03:51:59 UTC | 2026-07-01 03:52:16 UTC | 16.2s | `1.711` | `1.713` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0662 |
| 23 | `SHORT` | 2026-07-01 03:56:59 UTC | 2026-07-01 03:57:03 UTC | 3.5s | `1.712` | `1.710` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0666 |
| 24 | `LONG` | 2026-07-01 04:02:59 UTC | 2026-07-01 04:04:04 UTC | 1m 04s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0670 |
| 25 | `LONG` | 2026-07-01 04:11:59 UTC | 2026-07-01 04:16:02 UTC | 4m 02s | `1.700` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0674 |
| ... | ... | *(2192 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2218 | `LONG` | 2026-07-23 18:02:59 UTC | 2026-07-23 18:05:38 UTC | 2m 38s | `1.599` | `1.594` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.5%` | `STOP_LOSS_HIT` | $0.2012 |
| 2219 | `SHORT` | 2026-07-23 18:12:59 UTC | 2026-07-23 18:16:12 UTC | 3m 12s | `1.594` | `1.592` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2016 |
| 2220 | `SHORT` | 2026-07-23 18:17:59 UTC | 2026-07-23 18:18:03 UTC | 3.1s | `1.589` | `1.587` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2020 |
| 2221 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:30:28 UTC | 1m 28s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2024 |
| 2222 | `LONG` | 2026-07-23 18:35:59 UTC | 2026-07-23 18:42:33 UTC | 6m 33s | `1.610` | `1.605` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.2014 |
| 2223 | `LONG` | 2026-07-23 19:52:59 UTC | 2026-07-23 19:54:09 UTC | 1m 09s | `1.609` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2018 |
| 2224 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2022 |
| 2225 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 20:40:43 UTC | 12m 43s | `1.623` | `1.618` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.2012 |
| 2226 | `LONG` | 2026-07-23 20:45:59 UTC | 2026-07-23 20:46:24 UTC | 24.0s | `1.618` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2016 |
| 2227 | `SHORT` | 2026-07-23 20:52:59 UTC | 2026-07-23 21:04:40 UTC | 11m 40s | `1.621` | `1.626` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.2006 |
| 2228 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:07:45 UTC | 1m 45s | `1.622` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2010 |
| 2229 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:18:27 UTC | 27.3s | `1.617` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.2000 |
| 2230 | `LONG` | 2026-07-23 21:22:59 UTC | 2026-07-23 21:31:59 UTC | 8m 59s | `1.614` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.1990 |
| 2231 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:38:30 UTC | 30.0s | `1.603` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.1994 |
| 2232 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 21:56:25 UTC | 10m 25s | `1.605` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.4%` | `STOP_LOSS_HIT` | $0.1984 |
| 2233 | `SHORT` | 2026-07-23 22:00:59 UTC | 2026-07-23 22:02:05 UTC | 1m 05s | `1.609` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1988 |
| 2234 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:17 UTC | 5m 17s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1992 |
| 2235 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:24 UTC | 24.5s | `1.607` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1996 |
| 2236 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:20 UTC | 20.1s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2000 |
| 2237 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2004 |
| 2238 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:37:30 UTC | 2m 30s | `1.611` | `1.606` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.1994 |
| 2239 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:41:36 UTC | 37.0s | `1.604` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.1998 |
| 2240 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:35 UTC | 11m 35s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2002 |
| 2241 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:16:13 UTC | 7m 13s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2006 |
| 2242 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:05:13 UTC | 10m 13s | `1.599` | `1.594` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.5%` | `STOP_LOSS_HIT` | $0.1996 |

> 💡 *Full granular dataset with all 2242 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
