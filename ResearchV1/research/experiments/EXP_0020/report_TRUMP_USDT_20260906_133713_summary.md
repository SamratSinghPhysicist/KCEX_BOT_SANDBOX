# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:07:13 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.2096 USDT` | `₹19.80` | `+199.43%` |
| **Net Realized PnL** | **`+0.1396 USDT`** | **`₹+13.19`** | **`+199.43% Net ROI`** |
| **Gross Profit** | `+0.5476 USDT` | `₹51.72` | Total positive trade returns |
| **Gross Loss** | `-0.4080 USDT` | `₹38.54` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.34`** | — | Profitable |
| **Win / Loss Payoff** | `0.38` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0112 USDT` | `₹1.06` | **`-14.74%` Peak-to-Trough** |
| **Win Rate** | **`78.05%`** | — | `1369 Wins / 385 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `9.20` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `5.19` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `13.53` | — | Net ROI divided by Max Drawdown |

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
| **Directional Bias Policy** | `SHORT_ONLY` | Pre-trade signal directional allowance |

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
| **Total Trades Executed** | `1754` | Total completed trade lifecycle events |
| **Winning Trades** | `1369` | `78.05%` of total trades |
| **Losing Trades** | `385` | `21.95%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0001 USDT` (`₹+0.01`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0011 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #2 (SHORT) |
| **Largest Losing Trade** | `-0.0012 USDT (-27.0% ROE)` | Trade #1 (SHORT) |
| **Max Consecutive Wins** | `19` trades | Peak winning streak |
| **Max Consecutive Losses** | `5` trades | Peak losing streak |
| **Average Trade Duration** | `5m 10s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #1064 |
| **Longest Trade In-Position** | `1h 04m 03s` | Trade #836 |
| **Cumulative Time In Position** | `151h 20m 23s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `0` (0.0%) | `1754` (100.0%) | `1754` |
| **Wins / Losses** | `0 W / 0 L` | `1369 W / 385 L` | `1369 W / 385 L` |
| **Win Rate** | **`0.00%`** | **`78.05%`** | **`78.05%`** |
| **Gross Profit** | `+0.0000 USDT` | `+0.5476 USDT` | `+0.5476 USDT` |
| **Gross Loss** | `-0.0000 USDT` | `-0.4080 USDT` | `-0.4080 USDT` |
| **Net Realized PnL** | **`+0.0000 USDT`** | **`+0.1396 USDT`** | **`+0.1396 USDT`** |
| **Net PnL (INR)** | `₹+0.00` | `₹+13.19` | `₹+13.19` |
| **Profit Factor** | `0.00` | `1.34` | `1.34` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `STOP_LOSS_HIT` | `385` | `21.9%` | `-0.4080 USDT` | `₹-38.54` | `0.0%` | `8m 36s` |
| `MIN_PROFIT_TP_HIT` | `1369` | `78.1%` | `+0.5476 USDT` | `₹+51.72` | `100.0%` | `4m 12s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:52:46 UTC | 15m 46s | `1.664` | `1.670` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.0%` | `STOP_LOSS_HIT` | $0.0688 |
| 2 | `SHORT` | 2026-07-01 00:55:59 UTC | 2026-07-01 00:56:42 UTC | 42.7s | `1.669` | `1.667` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 3 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:23:12 UTC | 12.6s | `1.658` | `1.656` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 4 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:37:07 UTC | 2m 07s | `1.658` | `1.664` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.1%` | `STOP_LOSS_HIT` | $0.0684 |
| 5 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:09 UTC | 2m 09s | `1.676` | `1.674` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 6 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:02:52 UTC | 3m 52s | `1.678` | `1.684` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.8%` | `STOP_LOSS_HIT` | $0.0676 |
| 7 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:22:05 UTC | 4m 05s | `1.702` | `1.708` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0664 |
| 8 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:38 UTC | 38.4s | `1.704` | `1.710` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0652 |
| 9 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:24 UTC | 24.3s | `1.707` | `1.713` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0640 |
| 10 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:04 UTC | 4.8s | `1.729` | `1.727` | $0.35 | $0.00 | $0.000000 | **+0.0004** | `+8.7%` | `MIN_PROFIT_TP_HIT` | $0.0644 |
| 11 | `SHORT` | 2026-07-01 03:32:59 UTC | 2026-07-01 03:34:17 UTC | 1m 17s | `1.699` | `1.697` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0648 |
| 12 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:47:31 UTC | 5m 31s | `1.706` | `1.712` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0636 |
| 13 | `SHORT` | 2026-07-01 03:56:59 UTC | 2026-07-01 03:57:03 UTC | 3.5s | `1.712` | `1.710` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0640 |
| 14 | `SHORT` | 2026-07-01 04:21:59 UTC | 2026-07-01 04:23:55 UTC | 1m 55s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0644 |
| 15 | `SHORT` | 2026-07-01 04:59:59 UTC | 2026-07-01 05:00:10 UTC | 10.4s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0648 |
| 16 | `SHORT` | 2026-07-01 05:10:59 UTC | 2026-07-01 05:15:01 UTC | 4m 01s | `1.706` | `1.704` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 17 | `SHORT` | 2026-07-01 05:16:59 UTC | 2026-07-01 05:19:02 UTC | 2m 02s | `1.706` | `1.704` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0656 |
| 18 | `SHORT` | 2026-07-01 05:32:59 UTC | 2026-07-01 05:37:20 UTC | 4m 20s | `1.702` | `1.700` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0660 |
| 19 | `SHORT` | 2026-07-01 05:44:59 UTC | 2026-07-01 05:46:19 UTC | 1m 19s | `1.705` | `1.703` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0664 |
| 20 | `SHORT` | 2026-07-01 05:48:59 UTC | 2026-07-01 05:53:02 UTC | 4m 02s | `1.712` | `1.710` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 21 | `SHORT` | 2026-07-01 06:16:59 UTC | 2026-07-01 06:17:04 UTC | 4.8s | `1.710` | `1.708` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0672 |
| 22 | `SHORT` | 2026-07-01 06:55:59 UTC | 2026-07-01 06:56:34 UTC | 34.7s | `1.691` | `1.689` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0676 |
| 23 | `SHORT` | 2026-07-01 07:14:59 UTC | 2026-07-01 07:15:24 UTC | 24.5s | `1.690` | `1.688` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0680 |
| 24 | `SHORT` | 2026-07-01 07:26:59 UTC | 2026-07-01 07:27:17 UTC | 17.9s | `1.698` | `1.696` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 25 | `SHORT` | 2026-07-01 07:52:59 UTC | 2026-07-01 07:55:56 UTC | 2m 56s | `1.698` | `1.696` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| ... | ... | *(1704 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 1730 | `SHORT` | 2026-07-23 15:19:59 UTC | 2026-07-23 15:21:05 UTC | 1m 05s | `1.629` | `1.634` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-23.0%` | `STOP_LOSS_HIT` | $0.2084 |
| 1731 | `SHORT` | 2026-07-23 15:26:59 UTC | 2026-07-23 15:27:52 UTC | 52.5s | `1.631` | `1.629` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2088 |
| 1732 | `SHORT` | 2026-07-23 15:38:59 UTC | 2026-07-23 15:39:41 UTC | 41.7s | `1.635` | `1.633` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2092 |
| 1733 | `SHORT` | 2026-07-23 15:49:59 UTC | 2026-07-23 15:59:04 UTC | 9m 04s | `1.635` | `1.640` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.9%` | `STOP_LOSS_HIT` | $0.2082 |
| 1734 | `SHORT` | 2026-07-23 16:01:59 UTC | 2026-07-23 16:02:17 UTC | 17.5s | `1.638` | `1.643` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.9%` | `STOP_LOSS_HIT` | $0.2072 |
| 1735 | `SHORT` | 2026-07-23 16:17:59 UTC | 2026-07-23 16:18:39 UTC | 40.0s | `1.643` | `1.641` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.2076 |
| 1736 | `SHORT` | 2026-07-23 16:41:59 UTC | 2026-07-23 16:42:08 UTC | 8.3s | `1.637` | `1.635` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2080 |
| 1737 | `SHORT` | 2026-07-23 17:17:59 UTC | 2026-07-23 17:35:59 UTC | 17m 59s | `1.618` | `1.616` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2084 |
| 1738 | `SHORT` | 2026-07-23 17:47:59 UTC | 2026-07-23 17:53:13 UTC | 5m 13s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2088 |
| 1739 | `SHORT` | 2026-07-23 18:12:59 UTC | 2026-07-23 18:16:12 UTC | 3m 12s | `1.594` | `1.592` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2092 |
| 1740 | `SHORT` | 2026-07-23 18:17:59 UTC | 2026-07-23 18:18:03 UTC | 3.1s | `1.589` | `1.587` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2096 |
| 1741 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:30:28 UTC | 1m 28s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2100 |
| 1742 | `SHORT` | 2026-07-23 18:51:59 UTC | 2026-07-23 19:12:14 UTC | 20m 14s | `1.608` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.2090 |
| 1743 | `SHORT` | 2026-07-23 19:19:59 UTC | 2026-07-23 19:25:50 UTC | 5m 50s | `1.609` | `1.614` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.2080 |
| 1744 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:29:04 UTC | 4.2s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2084 |
| 1745 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2088 |
| 1746 | `SHORT` | 2026-07-23 20:52:59 UTC | 2026-07-23 21:04:40 UTC | 11m 40s | `1.621` | `1.626` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.2078 |
| 1747 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:07:45 UTC | 1m 45s | `1.622` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2082 |
| 1748 | `SHORT` | 2026-07-23 21:30:59 UTC | 2026-07-23 21:32:14 UTC | 1m 14s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2086 |
| 1749 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 21:56:25 UTC | 10m 25s | `1.605` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.4%` | `STOP_LOSS_HIT` | $0.2076 |
| 1750 | `SHORT` | 2026-07-23 22:00:59 UTC | 2026-07-23 22:02:05 UTC | 1m 05s | `1.609` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2080 |
| 1751 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:17 UTC | 5m 17s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2084 |
| 1752 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2088 |
| 1753 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:35 UTC | 11m 35s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2092 |
| 1754 | `SHORT` | 2026-07-23 23:19:59 UTC | 2026-07-23 23:47:35 UTC | 27m 35s | `1.606` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2096 |

> 💡 *Full granular dataset with all 1754 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
