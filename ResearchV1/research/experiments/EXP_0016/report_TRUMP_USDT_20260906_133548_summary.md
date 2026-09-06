# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:05:49 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.1300 USDT` | `₹12.28` | `+85.71%` |
| **Net Realized PnL** | **`+0.0600 USDT`** | **`₹+5.67`** | **`+85.71% Net ROI`** |
| **Gross Profit** | `+0.5248 USDT` | `₹49.57` | Total positive trade returns |
| **Gross Loss** | `-0.4648 USDT` | `₹43.90` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.13`** | — | Profitable |
| **Win / Loss Payoff** | `0.38` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0212 USDT` | `₹2.00` | **`-15.19%` Peak-to-Trough** |
| **Win Rate** | **`74.97%`** | — | `1312 Wins / 438 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `4.54` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `2.70` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `5.64` | — | Net ROI divided by Max Drawdown |

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
| **HTF Trend Baseline (200 EMA)** | `ENABLED` | Timeframe: `15m` / Period: `200` |
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
| **Total Trades Executed** | `1750` | Total completed trade lifecycle events |
| **Winning Trades** | `1312` | `74.97%` of total trades |
| **Losing Trades** | `438` | `25.03%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0011 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0012 USDT (-27.0% ROE)` | Trade #2 (SHORT) |
| **Max Consecutive Wins** | `25` trades | Peak winning streak |
| **Max Consecutive Losses** | `4` trades | Peak losing streak |
| **Average Trade Duration** | `5m 03s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #159 |
| **Longest Trade In-Position** | `1h 00m 46s` | Trade #840 |
| **Cumulative Time In Position** | `147h 44m 37s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `802` (45.8%) | `948` (54.2%) | `1750` |
| **Wins / Losses** | `580 W / 222 L` | `732 W / 216 L` | `1312 W / 438 L` |
| **Win Rate** | **`72.32%`** | **`77.22%`** | **`74.97%`** |
| **Gross Profit** | `+0.2320 USDT` | `+0.2928 USDT` | `+0.5248 USDT` |
| **Gross Loss** | `-0.2376 USDT` | `-0.2272 USDT` | `-0.4648 USDT` |
| **Net Realized PnL** | **`-0.0056 USDT`** | **`+0.0656 USDT`** | **`+0.0600 USDT`** |
| **Net PnL (INR)** | `₹-0.53` | `₹+6.20` | `₹+5.67` |
| **Profit Factor** | `0.98` | `1.29` | `1.13` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1312` | `75.0%` | `+0.5248 USDT` | `₹+49.57` | `100.0%` | `4m 06s` |
| `STOP_LOSS_HIT` | `438` | `25.0%` | `-0.4648 USDT` | `₹-43.90` | `0.0%` | `7m 57s` |

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
| 14 | `LONG` | 2026-07-01 02:22:59 UTC | 2026-07-01 02:23:01 UTC | 1.0s | `1.709` | `1.703` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.3%` | `STOP_LOSS_HIT` | $0.0660 |
| 15 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:13 UTC | 1m 13s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0664 |
| 16 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:05 UTC | 5.7s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 17 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:01 UTC | 3m 01s | `1.697` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0672 |
| 18 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:27 UTC | 28.0s | `1.711` | `1.705` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.3%` | `STOP_LOSS_HIT` | $0.0660 |
| 19 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:23:46 UTC | 3m 46s | `1.704` | `1.698` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0648 |
| 20 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:29:01 UTC | 1m 01s | `1.699` | `1.701` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 21 | `LONG` | 2026-07-01 03:51:59 UTC | 2026-07-01 03:52:16 UTC | 16.2s | `1.711` | `1.713` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0656 |
| 22 | `LONG` | 2026-07-01 04:02:59 UTC | 2026-07-01 04:04:04 UTC | 1m 04s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0660 |
| 23 | `LONG` | 2026-07-01 04:11:59 UTC | 2026-07-01 04:16:02 UTC | 4m 02s | `1.700` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0664 |
| 24 | `LONG` | 2026-07-01 04:27:59 UTC | 2026-07-01 04:31:23 UTC | 3m 23s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 25 | `LONG` | 2026-07-01 04:38:59 UTC | 2026-07-01 04:41:01 UTC | 2m 01s | `1.700` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0672 |
| ... | ... | *(1700 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 1726 | `LONG` | 2026-07-23 16:22:59 UTC | 2026-07-23 16:24:16 UTC | 1m 16s | `1.642` | `1.644` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.1358 |
| 1727 | `LONG` | 2026-07-23 16:34:59 UTC | 2026-07-23 16:36:24 UTC | 1m 24s | `1.639` | `1.641` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1362 |
| 1728 | `LONG` | 2026-07-23 16:37:59 UTC | 2026-07-23 16:40:30 UTC | 2m 30s | `1.641` | `1.636` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.9%` | `STOP_LOSS_HIT` | $0.1352 |
| 1729 | `LONG` | 2026-07-23 16:44:59 UTC | 2026-07-23 16:45:37 UTC | 37.1s | `1.637` | `1.632` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.9%` | `STOP_LOSS_HIT` | $0.1342 |
| 1730 | `LONG` | 2026-07-23 16:58:59 UTC | 2026-07-23 17:01:53 UTC | 2m 53s | `1.631` | `1.626` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-23.0%` | `STOP_LOSS_HIT` | $0.1332 |
| 1731 | `LONG` | 2026-07-23 17:04:59 UTC | 2026-07-23 17:05:31 UTC | 31.3s | `1.621` | `1.616` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.1322 |
| 1732 | `LONG` | 2026-07-23 17:08:59 UTC | 2026-07-23 17:09:17 UTC | 17.8s | `1.619` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1326 |
| 1733 | `LONG` | 2026-07-23 17:35:59 UTC | 2026-07-23 17:36:27 UTC | 27.0s | `1.616` | `1.618` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1330 |
| 1734 | `SHORT` | 2026-07-23 17:47:59 UTC | 2026-07-23 17:53:13 UTC | 5m 13s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1334 |
| 1735 | `SHORT` | 2026-07-23 18:12:59 UTC | 2026-07-23 18:16:12 UTC | 3m 12s | `1.594` | `1.592` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.1338 |
| 1736 | `SHORT` | 2026-07-23 18:17:59 UTC | 2026-07-23 18:18:03 UTC | 3.1s | `1.589` | `1.587` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.1342 |
| 1737 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:30:28 UTC | 1m 28s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1346 |
| 1738 | `SHORT` | 2026-07-23 18:51:59 UTC | 2026-07-23 19:12:14 UTC | 20m 14s | `1.608` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.1336 |
| 1739 | `LONG` | 2026-07-23 19:16:59 UTC | 2026-07-23 19:25:50 UTC | 8m 50s | `1.612` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1340 |
| 1740 | `LONG` | 2026-07-23 19:40:59 UTC | 2026-07-23 19:50:07 UTC | 9m 07s | `1.613` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.1330 |
| 1741 | `LONG` | 2026-07-23 20:16:59 UTC | 2026-07-23 20:24:57 UTC | 7m 57s | `1.625` | `1.620` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.1320 |
| 1742 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 20:40:43 UTC | 12m 43s | `1.623` | `1.618` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.1310 |
| 1743 | `LONG` | 2026-07-23 20:45:59 UTC | 2026-07-23 20:46:24 UTC | 24.0s | `1.618` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1314 |
| 1744 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:18:27 UTC | 27.3s | `1.617` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.1304 |
| 1745 | `LONG` | 2026-07-23 21:22:59 UTC | 2026-07-23 21:31:59 UTC | 8m 59s | `1.614` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.1294 |
| 1746 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 21:56:25 UTC | 10m 25s | `1.605` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.4%` | `STOP_LOSS_HIT` | $0.1284 |
| 1747 | `SHORT` | 2026-07-23 22:00:59 UTC | 2026-07-23 22:02:05 UTC | 1m 05s | `1.609` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1288 |
| 1748 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:17 UTC | 5m 17s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1292 |
| 1749 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:35 UTC | 11m 35s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1296 |
| 1750 | `SHORT` | 2026-07-23 23:19:59 UTC | 2026-07-23 23:47:35 UTC | 27m 35s | `1.606` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1300 |

> 💡 *Full granular dataset with all 1750 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
