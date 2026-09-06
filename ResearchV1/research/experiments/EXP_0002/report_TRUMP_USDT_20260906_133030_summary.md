# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:00:31 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.1240 USDT` | `₹11.71` | `+77.14%` |
| **Net Realized PnL** | **`+0.0540 USDT`** | **`₹+5.10`** | **`+77.14% Net ROI`** |
| **Gross Profit** | `+0.5288 USDT` | `₹49.95` | Total positive trade returns |
| **Gross Loss** | `-0.4748 USDT` | `₹44.84` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.11`** | — | Profitable |
| **Win / Loss Payoff** | `0.37` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0368 USDT` | `₹3.48` | **`-45.32%` Peak-to-Trough** |
| **Win Rate** | **`74.90%`** | — | `1322 Wins / 443 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `3.10` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `1.83` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `1.70` | — | Net ROI divided by Max Drawdown |

---

## 🛠️ Complete Configuration & Settings Used

### Strategy & Market Setup
| Configuration Setting | Value | Operational Details |
| :--- | :--- | :--- |
| **Trading Pair Symbol** | `TRUMP_USDT` | Base Asset: `TRUMP` / Quote Asset: `USDT` |
| **Candle Timeframe** | `1m` | Dynamic candle granularity evaluated by strategy indicators |
| **Strategy Evaluated** | `EMA_CROSSOVER` | EMA Crossover Trend Follower (Preset: 5/13 ; Closed Candle Confirmation: True) |
| **Strategy Preset** | `5/13` | Configured indicator preset profile |
| **Evaluation Date Range** | `2026-07-01` → `2026-07-24` | Historical evaluation window |
| **High-Fidelity Simulation** | `ENABLED (Tick Trades)` | Millisecond-level trade order matching & stop triggering |
| **Slippage Tolerance** | `0 ticks` (`0.000 USDT` per fill) | Adverse fill penalty applied to entry and exit orders |

### Strategy & Indicator Hyperparameters
| Hyperparameter | Value | Technical Context |
| :--- | :--- | :--- |
| **Active Strategy Engine** | `EMA_CROSSOVER` | Quantitative model evaluated |
| **Active Strategy Preset** | `5/13` | Selected preset configuration |
| **Fast EMA Period** | `5` | Short-term fast moving average |
| **Slow EMA Period** | `13` | Baseline slow moving average |
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
| **Total Trades Executed** | `1765` | Total completed trade lifecycle events |
| **Winning Trades** | `1322` | `74.90%` of total trades |
| **Losing Trades** | `443` | `25.10%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0011 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (SHORT) |
| **Largest Losing Trade** | `-0.0012 USDT (-26.5% ROE)` | Trade #6 (SHORT) |
| **Max Consecutive Wins** | `20` trades | Peak winning streak |
| **Max Consecutive Losses** | `4` trades | Peak losing streak |
| **Average Trade Duration** | `5m 02s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #578 |
| **Longest Trade In-Position** | `1h 27m 51s` | Trade #817 |
| **Cumulative Time In Position** | `148h 23m 34s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `892` (50.5%) | `873` (49.5%) | `1765` |
| **Wins / Losses** | `663 W / 229 L` | `659 W / 214 L` | `1322 W / 443 L` |
| **Win Rate** | **`74.33%`** | **`75.49%`** | **`74.90%`** |
| **Gross Profit** | `+0.2652 USDT` | `+0.2636 USDT` | `+0.5288 USDT` |
| **Gross Loss** | `-0.2462 USDT` | `-0.2286 USDT` | `-0.4748 USDT` |
| **Net Realized PnL** | **`+0.0190 USDT`** | **`+0.0350 USDT`** | **`+0.0540 USDT`** |
| **Net PnL (INR)** | `₹+1.79` | `₹+3.31` | `₹+5.10` |
| **Profit Factor** | `1.08` | `1.15` | `1.11` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1322` | `74.9%` | `+0.5288 USDT` | `₹+49.95` | `100.0%` | `4m 03s` |
| `STOP_LOSS_HIT` | `443` | `25.1%` | `-0.4748 USDT` | `₹-44.84` | `0.0%` | `8m 00s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `SHORT` | 2026-07-01 00:24:59 UTC | 2026-07-01 00:25:39 UTC | 39.9s | `1.660` | `1.658` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `LONG` | 2026-07-01 00:30:59 UTC | 2026-07-01 00:31:11 UTC | 11.9s | `1.665` | `1.667` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 3 | `SHORT` | 2026-07-01 00:49:59 UTC | 2026-07-01 00:51:03 UTC | 1m 03s | `1.667` | `1.665` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 4 | `SHORT` | 2026-07-01 01:05:59 UTC | 2026-07-01 01:07:03 UTC | 1m 03s | `1.663` | `1.661` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0716 |
| 5 | `LONG` | 2026-07-01 01:23:59 UTC | 2026-07-01 01:29:22 UTC | 5m 22s | `1.656` | `1.658` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0720 |
| 6 | `SHORT` | 2026-07-01 02:37:59 UTC | 2026-07-01 02:38:57 UTC | 57.2s | `1.696` | `1.702` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.5%` | `STOP_LOSS_HIT` | $0.0708 |
| 7 | `LONG` | 2026-07-01 02:58:59 UTC | 2026-07-01 03:00:56 UTC | 1m 56s | `1.702` | `1.704` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 8 | `SHORT` | 2026-07-01 03:16:59 UTC | 2026-07-01 03:17:03 UTC | 3.8s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0716 |
| 9 | `LONG` | 2026-07-01 03:38:59 UTC | 2026-07-01 03:39:14 UTC | 14.8s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0720 |
| 10 | `SHORT` | 2026-07-01 04:00:59 UTC | 2026-07-01 04:02:45 UTC | 1m 45s | `1.707` | `1.705` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0724 |
| 11 | `LONG` | 2026-07-01 04:20:59 UTC | 2026-07-01 04:22:31 UTC | 1m 31s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0728 |
| 12 | `SHORT` | 2026-07-01 04:36:59 UTC | 2026-07-01 04:37:14 UTC | 14.7s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0732 |
| 13 | `LONG` | 2026-07-01 04:57:59 UTC | 2026-07-01 05:06:16 UTC | 8m 16s | `1.703` | `1.705` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0736 |
| 14 | `SHORT` | 2026-07-01 05:22:59 UTC | 2026-07-01 05:26:59 UTC | 3m 59s | `1.701` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0740 |
| 15 | `LONG` | 2026-07-01 05:29:59 UTC | 2026-07-01 05:31:55 UTC | 1m 55s | `1.707` | `1.701` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0728 |
| 16 | `SHORT` | 2026-07-01 05:32:59 UTC | 2026-07-01 05:37:20 UTC | 4m 20s | `1.702` | `1.700` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0732 |
| 17 | `LONG` | 2026-07-01 05:45:59 UTC | 2026-07-01 05:48:36 UTC | 2m 36s | `1.706` | `1.708` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0736 |
| 18 | `SHORT` | 2026-07-01 06:03:59 UTC | 2026-07-01 06:14:55 UTC | 10m 55s | `1.705` | `1.711` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0724 |
| 19 | `SHORT` | 2026-07-01 06:19:59 UTC | 2026-07-01 06:21:46 UTC | 1m 46s | `1.705` | `1.703` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0728 |
| 20 | `LONG` | 2026-07-01 06:54:59 UTC | 2026-07-01 07:03:13 UTC | 8m 13s | `1.692` | `1.686` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.6%` | `STOP_LOSS_HIT` | $0.0716 |
| 21 | `SHORT` | 2026-07-01 07:04:59 UTC | 2026-07-01 07:05:24 UTC | 24.2s | `1.688` | `1.686` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0720 |
| 22 | `LONG` | 2026-07-01 07:13:59 UTC | 2026-07-01 07:14:30 UTC | 30.2s | `1.687` | `1.689` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0724 |
| 23 | `LONG` | 2026-07-01 07:17:59 UTC | 2026-07-01 07:21:39 UTC | 3m 39s | `1.690` | `1.692` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0728 |
| 24 | `SHORT` | 2026-07-01 07:41:59 UTC | 2026-07-01 07:44:13 UTC | 2m 13s | `1.695` | `1.693` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0732 |
| 25 | `LONG` | 2026-07-01 07:50:59 UTC | 2026-07-01 07:53:58 UTC | 2m 58s | `1.697` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0736 |
| ... | ... | *(1715 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 1741 | `SHORT` | 2026-07-23 15:28:59 UTC | 2026-07-23 15:30:31 UTC | 1m 31s | `1.630` | `1.628` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1200 |
| 1742 | `LONG` | 2026-07-23 15:33:59 UTC | 2026-07-23 15:35:02 UTC | 1m 02s | `1.633` | `1.635` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1204 |
| 1743 | `SHORT` | 2026-07-23 16:06:59 UTC | 2026-07-23 16:07:18 UTC | 18.6s | `1.636` | `1.634` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1208 |
| 1744 | `LONG` | 2026-07-23 16:12:59 UTC | 2026-07-23 16:13:11 UTC | 11.5s | `1.639` | `1.641` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1212 |
| 1745 | `SHORT` | 2026-07-23 16:31:59 UTC | 2026-07-23 16:35:09 UTC | 3m 09s | `1.640` | `1.638` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.1216 |
| 1746 | `LONG` | 2026-07-23 16:40:59 UTC | 2026-07-23 16:43:03 UTC | 2m 03s | `1.636` | `1.638` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1220 |
| 1747 | `LONG` | 2026-07-23 17:24:59 UTC | 2026-07-23 17:35:59 UTC | 10m 59s | `1.621` | `1.616` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.1210 |
| 1748 | `LONG` | 2026-07-23 18:22:59 UTC | 2026-07-23 18:25:10 UTC | 2m 10s | `1.600` | `1.602` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.1214 |
| 1749 | `SHORT` | 2026-07-23 18:43:59 UTC | 2026-07-23 18:49:06 UTC | 5m 06s | `1.605` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.4%` | `STOP_LOSS_HIT` | $0.1204 |
| 1750 | `SHORT` | 2026-07-23 19:07:59 UTC | 2026-07-23 19:08:33 UTC | 33.7s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1208 |
| 1751 | `SHORT` | 2026-07-23 19:09:59 UTC | 2026-07-23 19:10:50 UTC | 50.6s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1212 |
| 1752 | `SHORT` | 2026-07-23 19:11:59 UTC | 2026-07-23 19:19:32 UTC | 7m 32s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1216 |
| 1753 | `SHORT` | 2026-07-23 19:20:59 UTC | 2026-07-23 19:25:52 UTC | 4m 52s | `1.610` | `1.615` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.1206 |
| 1754 | `SHORT` | 2026-07-23 19:39:59 UTC | 2026-07-23 19:40:04 UTC | 4.8s | `1.615` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1210 |
| 1755 | `LONG` | 2026-07-23 19:58:59 UTC | 2026-07-23 19:59:12 UTC | 12.5s | `1.615` | `1.617` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1214 |
| 1756 | `SHORT` | 2026-07-23 20:25:59 UTC | 2026-07-23 20:40:29 UTC | 14m 29s | `1.621` | `1.619` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1218 |
| 1757 | `LONG` | 2026-07-23 20:53:59 UTC | 2026-07-23 20:55:28 UTC | 1m 28s | `1.621` | `1.623` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1222 |
| 1758 | `SHORT` | 2026-07-23 21:08:59 UTC | 2026-07-23 21:13:00 UTC | 4m 00s | `1.619` | `1.617` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1226 |
| 1759 | `LONG` | 2026-07-23 21:54:59 UTC | 2026-07-23 21:55:20 UTC | 20.1s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1230 |
| 1760 | `SHORT` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:21:20 UTC | 2m 20s | `1.607` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.1220 |
| 1761 | `LONG` | 2026-07-23 22:23:59 UTC | 2026-07-23 22:24:25 UTC | 25.1s | `1.615` | `1.617` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1224 |
| 1762 | `SHORT` | 2026-07-23 22:31:59 UTC | 2026-07-23 22:36:10 UTC | 4m 10s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1228 |
| 1763 | `LONG` | 2026-07-23 23:01:59 UTC | 2026-07-23 23:02:27 UTC | 27.6s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1232 |
| 1764 | `LONG` | 2026-07-23 23:17:59 UTC | 2026-07-23 23:22:40 UTC | 4m 40s | `1.606` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1236 |
| 1765 | `SHORT` | 2026-07-23 23:33:59 UTC | 2026-07-23 23:40:24 UTC | 6m 24s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1240 |

> 💡 *Full granular dataset with all 1765 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
