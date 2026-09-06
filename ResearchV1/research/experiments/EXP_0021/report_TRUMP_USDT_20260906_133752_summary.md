# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:07:52 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.1096 USDT` | `₹10.35` | `+56.57%` |
| **Net Realized PnL** | **`+0.0396 USDT`** | **`₹+3.74`** | **`+56.57% Net ROI`** |
| **Gross Profit** | `+0.2116 USDT` | `₹19.99` | Total positive trade returns |
| **Gross Loss** | `-0.1720 USDT` | `₹16.25` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.23`** | — | Profitable |
| **Win / Loss Payoff** | `0.38` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0084 USDT` | `₹0.79` | **`-7.89%` Peak-to-Trough** |
| **Win Rate** | **`76.45%`** | — | `529 Wins / 163 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `7.38` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `4.31` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `7.17` | — | Net ROI divided by Max Drawdown |

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
| **ADX Trend Regime Filter** | `ENABLED` | Period: `14` / Threshold: `25.0` |
| **HTF Trend Baseline (200 EMA)** | `ENABLED` | Timeframe: `15m` / Period: `200` |
| **Hourly Session Filter** | `ENABLED` | Blacklisted UTC Hours: `[2, 3, 4, 5, 17]` |
| **Directional Bias Policy** | `BOTH` | Pre-trade signal directional allowance |

### Position Sizing, Leverage & Risk Management
| Risk Parameter | Value | Operational Details |
| :--- | :--- | :--- |
| **Sizing Mode** | `MULTIPLIER` | Mode: `CONTRACTS`, `MULTIPLIER`, or `MIN` |
| **Trade Volume / Quantity** | `2x minimum volume (2 contract(s))` | Quantity committed per trade signal |
| **Leverage Multiplier** | `75x` | Margin required = Position Notional / Leverage |
| **Starting Capital** | `0.07 USDT` | `₹6.61 INR` (`1 USDT = ₹94.45`) |
| **Take Profit Target** | `+2 ticks` (`+0.002 USDT`) | Guaranteed Min-Profit TP (`entry + N*pu`) |
| **Stop Loss Rule** | `-25.0% ROE on committed margin` | Stop loss evaluation logic |

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
| **Total Trades Executed** | `692` | Total completed trade lifecycle events |
| **Winning Trades** | `529` | `76.45%` of total trades |
| **Losing Trades** | `163` | `23.55%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0001 USDT` (`₹+0.01`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0011 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.1% ROE)` | Trade #2 (LONG) |
| **Largest Losing Trade** | `-0.0012 USDT (-27.0% ROE)` | Trade #1 (SHORT) |
| **Max Consecutive Wins** | `22` trades | Peak winning streak |
| **Max Consecutive Losses** | `4` trades | Peak losing streak |
| **Average Trade Duration** | `5m 13s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.5s` | Trade #559 |
| **Longest Trade In-Position** | `1h 00m 46s` | Trade #314 |
| **Cumulative Time In Position** | `60h 21m 20s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `290` (41.9%) | `402` (58.1%) | `692` |
| **Wins / Losses** | `213 W / 77 L` | `316 W / 86 L` | `529 W / 163 L` |
| **Win Rate** | **`73.45%`** | **`78.61%`** | **`76.45%`** |
| **Gross Profit** | `+0.0852 USDT` | `+0.1264 USDT` | `+0.2116 USDT` |
| **Gross Loss** | `-0.0816 USDT` | `-0.0904 USDT` | `-0.1720 USDT` |
| **Net Realized PnL** | **`+0.0036 USDT`** | **`+0.0360 USDT`** | **`+0.0396 USDT`** |
| **Net PnL (INR)** | `₹+0.34` | `₹+3.40` | `₹+3.74` |
| **Profit Factor** | `1.04` | `1.40` | `1.23` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `STOP_LOSS_HIT` | `163` | `23.6%` | `-0.1720 USDT` | `₹-16.25` | `0.0%` | `8m 10s` |
| `MIN_PROFIT_TP_HIT` | `529` | `76.4%` | `+0.2116 USDT` | `₹+19.99` | `100.0%` | `4m 19s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:52:46 UTC | 15m 46s | `1.664` | `1.670` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.0%` | `STOP_LOSS_HIT` | $0.0688 |
| 2 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:03 UTC | 3.2s | `1.645` | `1.647` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 3 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:23:12 UTC | 12.6s | `1.658` | `1.656` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 4 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:09 UTC | 2m 09s | `1.676` | `1.674` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 5 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:10 UTC | 10.2s | `1.676` | `1.678` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 6 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:02:52 UTC | 3m 52s | `1.678` | `1.684` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.8%` | `STOP_LOSS_HIT` | $0.0692 |
| 7 | `LONG` | 2026-07-01 06:06:59 UTC | 2026-07-01 06:14:55 UTC | 7m 55s | `1.709` | `1.711` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 8 | `SHORT` | 2026-07-01 06:55:59 UTC | 2026-07-01 06:56:34 UTC | 34.7s | `1.691` | `1.689` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 9 | `SHORT` | 2026-07-01 08:39:59 UTC | 2026-07-01 08:47:15 UTC | 7m 15s | `1.689` | `1.687` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 10 | `LONG` | 2026-07-01 09:07:59 UTC | 2026-07-01 09:09:28 UTC | 1m 28s | `1.700` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 11 | `LONG` | 2026-07-01 09:25:59 UTC | 2026-07-01 09:32:33 UTC | 6m 33s | `1.711` | `1.705` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.3%` | `STOP_LOSS_HIT` | $0.0696 |
| 12 | `LONG` | 2026-07-01 09:34:59 UTC | 2026-07-01 09:46:42 UTC | 11m 42s | `1.704` | `1.698` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0684 |
| 13 | `SHORT` | 2026-07-01 10:24:59 UTC | 2026-07-01 10:25:52 UTC | 52.5s | `1.689` | `1.687` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 14 | `SHORT` | 2026-07-01 10:36:59 UTC | 2026-07-01 10:45:46 UTC | 8m 46s | `1.689` | `1.695` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.6%` | `STOP_LOSS_HIT` | $0.0676 |
| 15 | `SHORT` | 2026-07-01 12:18:59 UTC | 2026-07-01 12:19:25 UTC | 25.2s | `1.692` | `1.690` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0680 |
| 16 | `LONG` | 2026-07-01 16:52:59 UTC | 2026-07-01 16:53:22 UTC | 22.8s | `1.702` | `1.704` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 17 | `LONG` | 2026-07-01 18:04:59 UTC | 2026-07-01 18:14:08 UTC | 9m 08s | `1.716` | `1.718` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.7%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 18 | `LONG` | 2026-07-01 18:25:59 UTC | 2026-07-01 18:38:03 UTC | 12m 03s | `1.709` | `1.703` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.3%` | `STOP_LOSS_HIT` | $0.0676 |
| 19 | `LONG` | 2026-07-01 18:40:59 UTC | 2026-07-01 18:45:10 UTC | 4m 10s | `1.705` | `1.699` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0664 |
| 20 | `SHORT` | 2026-07-01 18:53:59 UTC | 2026-07-01 18:54:40 UTC | 40.9s | `1.693` | `1.691` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 21 | `SHORT` | 2026-07-01 19:06:59 UTC | 2026-07-01 19:08:13 UTC | 1m 13s | `1.697` | `1.695` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0672 |
| 22 | `SHORT` | 2026-07-01 19:09:59 UTC | 2026-07-01 19:11:35 UTC | 1m 35s | `1.695` | `1.693` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0676 |
| 23 | `SHORT` | 2026-07-01 20:49:59 UTC | 2026-07-01 21:09:16 UTC | 19m 16s | `1.691` | `1.697` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.6%` | `STOP_LOSS_HIT` | $0.0664 |
| 24 | `LONG` | 2026-07-01 21:20:59 UTC | 2026-07-01 21:21:35 UTC | 35.1s | `1.701` | `1.703` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 25 | `LONG` | 2026-07-01 21:24:59 UTC | 2026-07-01 21:26:02 UTC | 1m 02s | `1.703` | `1.705` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0672 |
| ... | ... | *(642 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 668 | `LONG` | 2026-07-23 07:40:59 UTC | 2026-07-23 07:46:04 UTC | 5m 04s | `1.622` | `1.624` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1084 |
| 669 | `LONG` | 2026-07-23 08:25:59 UTC | 2026-07-23 08:26:13 UTC | 13.5s | `1.636` | `1.638` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1088 |
| 670 | `LONG` | 2026-07-23 08:36:59 UTC | 2026-07-23 08:46:41 UTC | 9m 41s | `1.637` | `1.632` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.9%` | `STOP_LOSS_HIT` | $0.1078 |
| 671 | `LONG` | 2026-07-23 10:35:59 UTC | 2026-07-23 10:52:50 UTC | 16m 50s | `1.636` | `1.638` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1082 |
| 672 | `LONG` | 2026-07-23 11:32:59 UTC | 2026-07-23 11:34:24 UTC | 1m 24s | `1.644` | `1.646` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.1086 |
| 673 | `LONG` | 2026-07-23 12:04:59 UTC | 2026-07-23 12:06:36 UTC | 1m 36s | `1.648` | `1.650` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.1090 |
| 674 | `LONG` | 2026-07-23 12:28:59 UTC | 2026-07-23 12:30:50 UTC | 1m 50s | `1.649` | `1.651` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.1094 |
| 675 | `LONG` | 2026-07-23 12:42:59 UTC | 2026-07-23 12:43:06 UTC | 6.6s | `1.638` | `1.640` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1098 |
| 676 | `LONG` | 2026-07-23 12:49:59 UTC | 2026-07-23 12:50:49 UTC | 49.2s | `1.640` | `1.642` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.1102 |
| 677 | `LONG` | 2026-07-23 13:01:59 UTC | 2026-07-23 13:03:11 UTC | 1m 11s | `1.633` | `1.635` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1106 |
| 678 | `LONG` | 2026-07-23 13:04:59 UTC | 2026-07-23 13:05:38 UTC | 38.4s | `1.635` | `1.637` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1110 |
| 679 | `LONG` | 2026-07-23 15:11:59 UTC | 2026-07-23 15:13:01 UTC | 1m 01s | `1.628` | `1.630` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1114 |
| 680 | `LONG` | 2026-07-23 16:22:59 UTC | 2026-07-23 16:24:16 UTC | 1m 16s | `1.642` | `1.644` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.1118 |
| 681 | `SHORT` | 2026-07-23 18:12:59 UTC | 2026-07-23 18:16:12 UTC | 3m 12s | `1.594` | `1.592` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.1122 |
| 682 | `SHORT` | 2026-07-23 18:17:59 UTC | 2026-07-23 18:18:03 UTC | 3.1s | `1.589` | `1.587` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.1126 |
| 683 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:30:28 UTC | 1m 28s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1130 |
| 684 | `LONG` | 2026-07-23 20:16:59 UTC | 2026-07-23 20:24:57 UTC | 7m 57s | `1.625` | `1.620` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.1120 |
| 685 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 20:40:43 UTC | 12m 43s | `1.623` | `1.618` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.1110 |
| 686 | `LONG` | 2026-07-23 20:45:59 UTC | 2026-07-23 20:46:24 UTC | 24.0s | `1.618` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1114 |
| 687 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:18:27 UTC | 27.3s | `1.617` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.1104 |
| 688 | `LONG` | 2026-07-23 21:22:59 UTC | 2026-07-23 21:31:59 UTC | 8m 59s | `1.614` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.1094 |
| 689 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 21:56:25 UTC | 10m 25s | `1.605` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.4%` | `STOP_LOSS_HIT` | $0.1084 |
| 690 | `SHORT` | 2026-07-23 22:00:59 UTC | 2026-07-23 22:02:05 UTC | 1m 05s | `1.609` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1088 |
| 691 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:17 UTC | 5m 17s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1092 |
| 692 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:35 UTC | 11m 35s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1096 |

> 💡 *Full granular dataset with all 692 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
