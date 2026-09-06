# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:15:18 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.1342 USDT` | `₹12.68` | `+91.71%` |
| **Net Realized PnL** | **`+0.0642 USDT`** | **`₹+6.06`** | **`+91.71% Net ROI`** |
| **Gross Profit** | `+0.5332 USDT` | `₹50.36` | Total positive trade returns |
| **Gross Loss** | `-0.4690 USDT` | `₹44.30` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.14`** | — | Profitable |
| **Win / Loss Payoff** | `0.40` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0292 USDT` | `₹2.76` | **`-36.41%` Peak-to-Trough** |
| **Win Rate** | **`73.97%`** | — | `1333 Wins / 469 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `3.84` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `2.35` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `2.52` | — | Net ROI divided by Max Drawdown |

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
| **Total Trades Executed** | `1802` | Total completed trade lifecycle events |
| **Winning Trades** | `1333` | `73.97%` of total trades |
| **Losing Trades** | `469` | `26.03%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0010 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (SHORT) |
| **Largest Losing Trade** | `-0.0010 USDT (-22.1% ROE)` | Trade #6 (SHORT) |
| **Max Consecutive Wins** | `20` trades | Peak winning streak |
| **Max Consecutive Losses** | `4` trades | Peak losing streak |
| **Average Trade Duration** | `4m 48s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #615 |
| **Longest Trade In-Position** | `1h 27m 51s` | Trade #854 |
| **Cumulative Time In Position** | `144h 15m 41s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `910` (50.5%) | `892` (49.5%) | `1802` |
| **Wins / Losses** | `667 W / 243 L` | `666 W / 226 L` | `1333 W / 469 L` |
| **Win Rate** | **`73.30%`** | **`74.66%`** | **`73.97%`** |
| **Gross Profit** | `+0.2668 USDT` | `+0.2664 USDT` | `+0.5332 USDT` |
| **Gross Loss** | `-0.2430 USDT` | `-0.2260 USDT` | `-0.4690 USDT` |
| **Net Realized PnL** | **`+0.0238 USDT`** | **`+0.0404 USDT`** | **`+0.0642 USDT`** |
| **Net PnL (INR)** | `₹+2.25` | `₹+3.82` | `₹+6.06` |
| **Profit Factor** | `1.10` | `1.18` | `1.14` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1333` | `74.0%` | `+0.5332 USDT` | `₹+50.36` | `100.0%` | `3m 54s` |
| `STOP_LOSS_HIT` | `469` | `26.0%` | `-0.4690 USDT` | `₹-44.30` | `0.0%` | `7m 19s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `SHORT` | 2026-07-01 00:24:59 UTC | 2026-07-01 00:25:39 UTC | 39.9s | `1.660` | `1.658` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `LONG` | 2026-07-01 00:30:59 UTC | 2026-07-01 00:31:11 UTC | 11.9s | `1.665` | `1.667` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 3 | `SHORT` | 2026-07-01 00:49:59 UTC | 2026-07-01 00:51:03 UTC | 1m 03s | `1.667` | `1.665` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 4 | `SHORT` | 2026-07-01 01:05:59 UTC | 2026-07-01 01:07:03 UTC | 1m 03s | `1.663` | `1.661` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0716 |
| 5 | `LONG` | 2026-07-01 01:23:59 UTC | 2026-07-01 01:29:22 UTC | 5m 22s | `1.656` | `1.658` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0720 |
| 6 | `SHORT` | 2026-07-01 02:37:59 UTC | 2026-07-01 02:38:35 UTC | 35.3s | `1.696` | `1.701` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.1%` | `STOP_LOSS_HIT` | $0.0710 |
| 7 | `LONG` | 2026-07-01 02:58:59 UTC | 2026-07-01 03:00:56 UTC | 1m 56s | `1.702` | `1.704` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0714 |
| 8 | `SHORT` | 2026-07-01 03:16:59 UTC | 2026-07-01 03:17:03 UTC | 3.8s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0718 |
| 9 | `LONG` | 2026-07-01 03:38:59 UTC | 2026-07-01 03:39:14 UTC | 14.8s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0722 |
| 10 | `SHORT` | 2026-07-01 04:00:59 UTC | 2026-07-01 04:02:45 UTC | 1m 45s | `1.707` | `1.705` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0726 |
| 11 | `LONG` | 2026-07-01 04:20:59 UTC | 2026-07-01 04:22:31 UTC | 1m 31s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0730 |
| 12 | `SHORT` | 2026-07-01 04:36:59 UTC | 2026-07-01 04:37:14 UTC | 14.7s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0734 |
| 13 | `LONG` | 2026-07-01 04:57:59 UTC | 2026-07-01 05:06:16 UTC | 8m 16s | `1.703` | `1.705` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0738 |
| 14 | `SHORT` | 2026-07-01 05:22:59 UTC | 2026-07-01 05:26:59 UTC | 3m 59s | `1.701` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0742 |
| 15 | `LONG` | 2026-07-01 05:29:59 UTC | 2026-07-01 05:30:34 UTC | 34.1s | `1.707` | `1.702` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0732 |
| 16 | `SHORT` | 2026-07-01 05:32:59 UTC | 2026-07-01 05:37:20 UTC | 4m 20s | `1.702` | `1.700` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0736 |
| 17 | `LONG` | 2026-07-01 05:45:59 UTC | 2026-07-01 05:48:36 UTC | 2m 36s | `1.706` | `1.708` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0740 |
| 18 | `SHORT` | 2026-07-01 06:03:59 UTC | 2026-07-01 06:05:28 UTC | 1m 28s | `1.705` | `1.710` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0730 |
| 19 | `LONG` | 2026-07-01 06:14:59 UTC | 2026-07-01 06:18:13 UTC | 3m 13s | `1.711` | `1.706` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-21.9%` | `STOP_LOSS_HIT` | $0.0720 |
| 20 | `SHORT` | 2026-07-01 06:19:59 UTC | 2026-07-01 06:21:46 UTC | 1m 46s | `1.705` | `1.703` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0724 |
| 21 | `LONG` | 2026-07-01 06:54:59 UTC | 2026-07-01 07:03:03 UTC | 8m 03s | `1.692` | `1.687` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.2%` | `STOP_LOSS_HIT` | $0.0714 |
| 22 | `SHORT` | 2026-07-01 07:04:59 UTC | 2026-07-01 07:05:24 UTC | 24.2s | `1.688` | `1.686` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0718 |
| 23 | `LONG` | 2026-07-01 07:13:59 UTC | 2026-07-01 07:14:30 UTC | 30.2s | `1.687` | `1.689` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0722 |
| 24 | `LONG` | 2026-07-01 07:17:59 UTC | 2026-07-01 07:21:39 UTC | 3m 39s | `1.690` | `1.692` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0726 |
| 25 | `SHORT` | 2026-07-01 07:41:59 UTC | 2026-07-01 07:44:13 UTC | 2m 13s | `1.695` | `1.693` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0730 |
| ... | ... | *(1752 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 1778 | `SHORT` | 2026-07-23 15:28:59 UTC | 2026-07-23 15:30:31 UTC | 1m 31s | `1.630` | `1.628` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1302 |
| 1779 | `LONG` | 2026-07-23 15:33:59 UTC | 2026-07-23 15:35:02 UTC | 1m 02s | `1.633` | `1.635` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1306 |
| 1780 | `SHORT` | 2026-07-23 16:06:59 UTC | 2026-07-23 16:07:18 UTC | 18.6s | `1.636` | `1.634` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1310 |
| 1781 | `LONG` | 2026-07-23 16:12:59 UTC | 2026-07-23 16:13:11 UTC | 11.5s | `1.639` | `1.641` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1314 |
| 1782 | `SHORT` | 2026-07-23 16:31:59 UTC | 2026-07-23 16:35:09 UTC | 3m 09s | `1.640` | `1.638` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.1318 |
| 1783 | `LONG` | 2026-07-23 16:40:59 UTC | 2026-07-23 16:43:03 UTC | 2m 03s | `1.636` | `1.638` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1322 |
| 1784 | `LONG` | 2026-07-23 17:24:59 UTC | 2026-07-23 17:35:59 UTC | 10m 59s | `1.621` | `1.616` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.1312 |
| 1785 | `LONG` | 2026-07-23 18:22:59 UTC | 2026-07-23 18:25:10 UTC | 2m 10s | `1.600` | `1.602` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.1316 |
| 1786 | `SHORT` | 2026-07-23 18:43:59 UTC | 2026-07-23 18:49:06 UTC | 5m 06s | `1.605` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.4%` | `STOP_LOSS_HIT` | $0.1306 |
| 1787 | `SHORT` | 2026-07-23 19:07:59 UTC | 2026-07-23 19:08:33 UTC | 33.7s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1310 |
| 1788 | `SHORT` | 2026-07-23 19:09:59 UTC | 2026-07-23 19:10:50 UTC | 50.6s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1314 |
| 1789 | `SHORT` | 2026-07-23 19:11:59 UTC | 2026-07-23 19:19:32 UTC | 7m 32s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1318 |
| 1790 | `SHORT` | 2026-07-23 19:20:59 UTC | 2026-07-23 19:25:52 UTC | 4m 52s | `1.610` | `1.615` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.1308 |
| 1791 | `SHORT` | 2026-07-23 19:39:59 UTC | 2026-07-23 19:40:04 UTC | 4.8s | `1.615` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1312 |
| 1792 | `LONG` | 2026-07-23 19:58:59 UTC | 2026-07-23 19:59:12 UTC | 12.5s | `1.615` | `1.617` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1316 |
| 1793 | `SHORT` | 2026-07-23 20:25:59 UTC | 2026-07-23 20:40:29 UTC | 14m 29s | `1.621` | `1.619` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1320 |
| 1794 | `LONG` | 2026-07-23 20:53:59 UTC | 2026-07-23 20:55:28 UTC | 1m 28s | `1.621` | `1.623` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1324 |
| 1795 | `SHORT` | 2026-07-23 21:08:59 UTC | 2026-07-23 21:13:00 UTC | 4m 00s | `1.619` | `1.617` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1328 |
| 1796 | `LONG` | 2026-07-23 21:54:59 UTC | 2026-07-23 21:55:20 UTC | 20.1s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1332 |
| 1797 | `SHORT` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:21:20 UTC | 2m 20s | `1.607` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.1322 |
| 1798 | `LONG` | 2026-07-23 22:23:59 UTC | 2026-07-23 22:24:25 UTC | 25.1s | `1.615` | `1.617` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1326 |
| 1799 | `SHORT` | 2026-07-23 22:31:59 UTC | 2026-07-23 22:36:10 UTC | 4m 10s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1330 |
| 1800 | `LONG` | 2026-07-23 23:01:59 UTC | 2026-07-23 23:02:27 UTC | 27.6s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1334 |
| 1801 | `LONG` | 2026-07-23 23:17:59 UTC | 2026-07-23 23:22:40 UTC | 4m 40s | `1.606` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1338 |
| 1802 | `SHORT` | 2026-07-23 23:33:59 UTC | 2026-07-23 23:40:24 UTC | 6m 24s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1342 |

> 💡 *Full granular dataset with all 1802 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
