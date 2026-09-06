# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:18:03 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.0918 USDT` | `₹8.67` | `+31.14%` |
| **Net Realized PnL** | **`+0.0218 USDT`** | **`₹+2.06`** | **`+31.14% Net ROI`** |
| **Gross Profit** | `+0.3828 USDT` | `₹36.16` | Total positive trade returns |
| **Gross Loss** | `-0.3610 USDT` | `₹34.10` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.06`** | — | Profitable |
| **Win / Loss Payoff** | `0.40` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0276 USDT` | `₹2.61` | **`-25.14%` Peak-to-Trough** |
| **Win Rate** | **`72.61%`** | — | `957 Wins / 361 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `2.61` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `1.63` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `1.24` | — | Net ROI divided by Max Drawdown |

---

## 🛠️ Complete Configuration & Settings Used

### Strategy & Market Setup
| Configuration Setting | Value | Operational Details |
| :--- | :--- | :--- |
| **Trading Pair Symbol** | `TRUMP_USDT` | Base Asset: `TRUMP` / Quote Asset: `USDT` |
| **Candle Timeframe** | `1m` | Dynamic candle granularity evaluated by strategy indicators |
| **Strategy Evaluated** | `EMA_CROSSOVER` | EMA Crossover Trend Follower (Preset: 5/13 ; Closed Candle Confirmation: True) |
| **Strategy Preset** | `5/13` | Configured indicator preset profile |
| **Evaluation Date Range** | `2026-08-16` → `2026-08-31` | Historical evaluation window |
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
| **Total Trades Executed** | `1318` | Total completed trade lifecycle events |
| **Winning Trades** | `957` | `72.61%` of total trades |
| **Losing Trades** | `361` | `27.39%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0010 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+5.0% ROE)` | Trade #442 (SHORT) |
| **Largest Losing Trade** | `-0.0010 USDT (-16.3% ROE)` | Trade #432 (SHORT) |
| **Max Consecutive Wins** | `20` trades | Peak winning streak |
| **Max Consecutive Losses** | `5` trades | Peak losing streak |
| **Average Trade Duration** | `2m 10s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #436 |
| **Longest Trade In-Position** | `1h 45m 29s` | Trade #189 |
| **Cumulative Time In Position** | `47h 45m 38s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `672` (51.0%) | `646` (49.0%) | `1318` |
| **Wins / Losses** | `476 W / 196 L` | `481 W / 165 L` | `957 W / 361 L` |
| **Win Rate** | **`70.83%`** | **`74.46%`** | **`72.61%`** |
| **Gross Profit** | `+0.1904 USDT` | `+0.1924 USDT` | `+0.3828 USDT` |
| **Gross Loss** | `-0.1960 USDT` | `-0.1650 USDT` | `-0.3610 USDT` |
| **Net Realized PnL** | **`-0.0056 USDT`** | **`+0.0274 USDT`** | **`+0.0218 USDT`** |
| **Net PnL (INR)** | `₹-0.53` | `₹+2.59` | `₹+2.06` |
| **Profit Factor** | `0.97` | `1.17` | `1.06` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `957` | `72.6%` | `+0.3828 USDT` | `₹+36.16` | `100.0%` | `1m 55s` |
| `STOP_LOSS_HIT` | `361` | `27.4%` | `-0.3610 USDT` | `₹-34.10` | `0.0%` | `2m 50s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `SHORT` | 2026-08-16 00:41:59 UTC | 2026-08-16 00:49:08 UTC | 7m 08s | `1.409` | `1.407` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.6%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `LONG` | 2026-08-16 00:54:59 UTC | 2026-08-16 00:56:17 UTC | 1m 17s | `1.409` | `1.411` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.6%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 3 | `SHORT` | 2026-08-16 01:10:59 UTC | 2026-08-16 01:13:56 UTC | 2m 56s | `1.405` | `1.403` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 4 | `LONG` | 2026-08-16 01:46:59 UTC | 2026-08-16 02:10:43 UTC | 23m 43s | `1.396` | `1.391` | $0.28 | $0.00 | $0.000000 | **-0.0010** | `-26.9%` | `STOP_LOSS_HIT` | $0.0702 |
| 5 | `LONG` | 2026-08-16 02:22:59 UTC | 2026-08-16 02:25:21 UTC | 2m 21s | `1.394` | `1.396` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 6 | `SHORT` | 2026-08-16 02:39:59 UTC | 2026-08-16 02:51:15 UTC | 11m 15s | `1.394` | `1.392` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0710 |
| 7 | `LONG` | 2026-08-16 03:04:59 UTC | 2026-08-16 03:11:46 UTC | 6m 46s | `1.394` | `1.396` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0714 |
| 8 | `SHORT` | 2026-08-16 03:14:59 UTC | 2026-08-16 03:30:45 UTC | 15m 45s | `1.392` | `1.397` | $0.28 | $0.00 | $0.000000 | **-0.0010** | `-26.9%` | `STOP_LOSS_HIT` | $0.0704 |
| 9 | `SHORT` | 2026-08-16 03:43:59 UTC | 2026-08-16 03:47:55 UTC | 3m 55s | `1.396` | `1.394` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 10 | `SHORT` | 2026-08-16 03:48:59 UTC | 2026-08-16 04:00:05 UTC | 11m 05s | `1.394` | `1.392` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 11 | `LONG` | 2026-08-16 04:06:59 UTC | 2026-08-16 04:25:54 UTC | 18m 54s | `1.392` | `1.394` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0716 |
| 12 | `SHORT` | 2026-08-16 04:56:59 UTC | 2026-08-16 04:58:08 UTC | 1m 08s | `1.398` | `1.396` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0720 |
| 13 | `LONG` | 2026-08-16 05:04:59 UTC | 2026-08-16 05:10:31 UTC | 5m 31s | `1.398` | `1.400` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0724 |
| 14 | `SHORT` | 2026-08-16 05:15:59 UTC | 2026-08-16 05:18:43 UTC | 2m 43s | `1.398` | `1.396` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0728 |
| 15 | `LONG` | 2026-08-16 05:26:59 UTC | 2026-08-16 05:39:18 UTC | 12m 18s | `1.398` | `1.400` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0732 |
| 16 | `SHORT` | 2026-08-16 05:47:59 UTC | 2026-08-16 05:48:20 UTC | 20.4s | `1.399` | `1.397` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0736 |
| 17 | `SHORT` | 2026-08-16 05:49:59 UTC | 2026-08-16 05:55:02 UTC | 5m 02s | `1.397` | `1.395` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0740 |
| 18 | `LONG` | 2026-08-16 06:09:59 UTC | 2026-08-16 06:42:47 UTC | 32m 47s | `1.397` | `1.392` | $0.28 | $0.00 | $0.000000 | **-0.0010** | `-26.8%` | `STOP_LOSS_HIT` | $0.0730 |
| 19 | `LONG` | 2026-08-16 06:49:59 UTC | 2026-08-16 07:00:29 UTC | 10m 29s | `1.392` | `1.394` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0734 |
| 20 | `LONG` | 2026-08-16 07:07:59 UTC | 2026-08-16 07:11:50 UTC | 3m 50s | `1.392` | `1.394` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0738 |
| 21 | `SHORT` | 2026-08-16 07:42:59 UTC | 2026-08-16 07:43:25 UTC | 25.2s | `1.399` | `1.397` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0742 |
| 22 | `SHORT` | 2026-08-16 07:44:59 UTC | 2026-08-16 08:32:15 UTC | 47m 15s | `1.396` | `1.394` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0746 |
| 23 | `LONG` | 2026-08-16 08:49:59 UTC | 2026-08-16 08:56:31 UTC | 6m 31s | `1.396` | `1.398` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0750 |
| 24 | `SHORT` | 2026-08-16 09:10:59 UTC | 2026-08-16 09:14:22 UTC | 3m 22s | `1.396` | `1.394` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0754 |
| 25 | `LONG` | 2026-08-16 09:39:59 UTC | 2026-08-16 10:28:14 UTC | 48m 14s | `1.394` | `1.389` | $0.28 | $0.00 | $0.000000 | **-0.0010** | `-26.9%` | `STOP_LOSS_HIT` | $0.0744 |
| ... | ... | *(1268 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 1294 | `SHORT` | 2026-08-30 17:13:59 UTC | 2026-08-30 17:14:06 UTC | 6.5s | `2.575` | `2.573` | $0.52 | $0.01 | $0.000000 | **+0.0004** | `+5.8%` | `MIN_PROFIT_TP_HIT` | $0.0878 |
| 1295 | `LONG` | 2026-08-30 17:15:59 UTC | 2026-08-30 17:16:00 UTC | 0.5s | `2.567` | `2.569` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.8%` | `MIN_PROFIT_TP_HIT` | $0.0882 |
| 1296 | `LONG` | 2026-08-30 17:40:59 UTC | 2026-08-30 17:41:54 UTC | 54.1s | `2.549` | `2.551` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.0886 |
| 1297 | `LONG` | 2026-08-30 17:42:59 UTC | 2026-08-30 17:45:01 UTC | 2m 01s | `2.551` | `2.553` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.0890 |
| 1298 | `SHORT` | 2026-08-30 17:47:59 UTC | 2026-08-30 17:48:05 UTC | 5.1s | `2.546` | `2.544` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.0894 |
| 1299 | `LONG` | 2026-08-30 17:59:59 UTC | 2026-08-30 18:01:02 UTC | 1m 02s | `2.543` | `2.545` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.0898 |
| 1300 | `SHORT` | 2026-08-30 18:07:59 UTC | 2026-08-30 18:10:24 UTC | 2m 24s | `2.539` | `2.537` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.0902 |
| 1301 | `LONG` | 2026-08-30 18:15:59 UTC | 2026-08-30 18:16:51 UTC | 51.9s | `2.540` | `2.535` | $0.51 | $0.01 | $0.000000 | **-0.0010** | `-14.8%` | `STOP_LOSS_HIT` | $0.0892 |
| 1302 | `SHORT` | 2026-08-30 18:17:59 UTC | 2026-08-30 18:20:27 UTC | 2m 27s | `2.534` | `2.539` | $0.51 | $0.01 | $0.000000 | **-0.0010** | `-14.8%` | `STOP_LOSS_HIT` | $0.0882 |
| 1303 | `LONG` | 2026-08-30 18:26:59 UTC | 2026-08-30 18:27:14 UTC | 14.8s | `2.541` | `2.543` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.0886 |
| 1304 | `SHORT` | 2026-08-30 18:48:59 UTC | 2026-08-30 18:51:10 UTC | 2m 10s | `2.549` | `2.554` | $0.51 | $0.01 | $0.000000 | **-0.0010** | `-14.7%` | `STOP_LOSS_HIT` | $0.0876 |
| 1305 | `LONG` | 2026-08-30 19:13:59 UTC | 2026-08-30 19:14:11 UTC | 11.1s | `2.554` | `2.549` | $0.51 | $0.01 | $0.000000 | **-0.0010** | `-14.7%` | `STOP_LOSS_HIT` | $0.0866 |
| 1306 | `SHORT` | 2026-08-30 19:21:59 UTC | 2026-08-30 19:22:59 UTC | 59.1s | `2.543` | `2.541` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.0870 |
| 1307 | `LONG` | 2026-08-30 19:53:59 UTC | 2026-08-30 19:54:11 UTC | 11.7s | `2.526` | `2.528` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.0874 |
| 1308 | `SHORT` | 2026-08-30 20:09:59 UTC | 2026-08-30 20:10:14 UTC | 14.0s | `2.535` | `2.533` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.0878 |
| 1309 | `SHORT` | 2026-08-30 20:29:59 UTC | 2026-08-30 20:30:03 UTC | 3.6s | `2.529` | `2.527` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.0882 |
| 1310 | `LONG` | 2026-08-30 20:49:59 UTC | 2026-08-30 20:50:19 UTC | 19.8s | `2.520` | `2.522` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.0886 |
| 1311 | `SHORT` | 2026-08-30 20:59:59 UTC | 2026-08-30 21:00:38 UTC | 38.6s | `2.515` | `2.513` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.0890 |
| 1312 | `LONG` | 2026-08-30 21:29:59 UTC | 2026-08-30 21:30:14 UTC | 15.0s | `2.503` | `2.505` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.0894 |
| 1313 | `SHORT` | 2026-08-30 21:42:59 UTC | 2026-08-30 21:43:55 UTC | 55.0s | `2.496` | `2.494` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.0898 |
| 1314 | `LONG` | 2026-08-30 21:55:59 UTC | 2026-08-30 21:56:08 UTC | 8.4s | `2.505` | `2.507` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.0902 |
| 1315 | `SHORT` | 2026-08-30 22:12:59 UTC | 2026-08-30 22:13:59 UTC | 59.4s | `2.504` | `2.502` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.0906 |
| 1316 | `LONG` | 2026-08-30 23:16:59 UTC | 2026-08-30 23:17:00 UTC | 0.5s | `2.417` | `2.419` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.0910 |
| 1317 | `SHORT` | 2026-08-30 23:28:59 UTC | 2026-08-30 23:29:03 UTC | 3.3s | `2.401` | `2.399` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.0914 |
| 1318 | `LONG` | 2026-08-30 23:56:59 UTC | 2026-08-30 23:57:04 UTC | 4.9s | `2.342` | `2.344` | $0.47 | $0.01 | $0.000000 | **+0.0004** | `+6.4%` | `MIN_PROFIT_TP_HIT` | $0.0918 |

> 💡 *Full granular dataset with all 1318 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
