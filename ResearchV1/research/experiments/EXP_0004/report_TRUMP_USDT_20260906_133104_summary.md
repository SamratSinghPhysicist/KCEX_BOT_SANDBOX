# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:01:04 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.0672 USDT` | `₹6.35` | `-4.00%` |
| **Net Realized PnL** | **`-0.0028 USDT`** | **`₹-0.26`** | **`-4.00% Net ROI`** |
| **Gross Profit** | `+0.4816 USDT` | `₹45.49` | Total positive trade returns |
| **Gross Loss** | `-0.4844 USDT` | `₹45.75` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`0.99`** | — | Unprofitable / Needs Optimization |
| **Win / Loss Payoff** | `1.00` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0212 USDT` | `₹2.00` | **`-29.44%` Peak-to-Trough** |
| **Win Rate** | **`49.86%`** | — | `1204 Wins / 1211 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `0.06` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `0.06` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `-0.14` | — | Net ROI divided by Max Drawdown |

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
| **Stop Loss Rule** | `-2 ticks away from entry (0.002 USDT)` | Stop loss evaluation logic |

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
| **Total Trades Executed** | `2415` | Total completed trade lifecycle events |
| **Winning Trades** | `1204` | `49.86%` of total trades |
| **Losing Trades** | `1211` | `50.14%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `-0.0000 USDT` (`₹-0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0004 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (SHORT) |
| **Largest Losing Trade** | `-0.0004 USDT (-9.0% ROE)` | Trade #4 (SHORT) |
| **Max Consecutive Wins** | `9` trades | Peak winning streak |
| **Max Consecutive Losses** | `9` trades | Peak losing streak |
| **Average Trade Duration** | `1m 44s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #86 |
| **Longest Trade In-Position** | `23m 49s` | Trade #1418 |
| **Cumulative Time In Position** | `70h 24m 14s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1221` (50.6%) | `1194` (49.4%) | `2415` |
| **Wins / Losses** | `594 W / 627 L` | `610 W / 584 L` | `1204 W / 1211 L` |
| **Win Rate** | **`48.65%`** | **`51.09%`** | **`49.86%`** |
| **Gross Profit** | `+0.2376 USDT` | `+0.2440 USDT` | `+0.4816 USDT` |
| **Gross Loss** | `-0.2508 USDT` | `-0.2336 USDT` | `-0.4844 USDT` |
| **Net Realized PnL** | **`-0.0132 USDT`** | **`+0.0104 USDT`** | **`-0.0028 USDT`** |
| **Net PnL (INR)** | `₹-1.25` | `₹+0.98` | `₹-0.26` |
| **Profit Factor** | `0.95` | `1.04` | `0.99` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1204` | `49.9%` | `+0.4816 USDT` | `₹+45.49` | `100.0%` | `1m 44s` |
| `STOP_LOSS_HIT` | `1211` | `50.1%` | `-0.4844 USDT` | `₹-45.75` | `0.0%` | `1m 45s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `SHORT` | 2026-07-01 00:24:59 UTC | 2026-07-01 00:25:39 UTC | 39.9s | `1.660` | `1.658` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `LONG` | 2026-07-01 00:30:59 UTC | 2026-07-01 00:31:11 UTC | 11.9s | `1.665` | `1.667` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 3 | `SHORT` | 2026-07-01 00:49:59 UTC | 2026-07-01 00:51:03 UTC | 1m 03s | `1.667` | `1.665` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 4 | `SHORT` | 2026-07-01 01:05:59 UTC | 2026-07-01 01:06:03 UTC | 3.7s | `1.663` | `1.665` | $0.33 | $0.00 | $0.000000 | **-0.0004** | `-9.0%` | `STOP_LOSS_HIT` | $0.0708 |
| 5 | `LONG` | 2026-07-01 01:23:59 UTC | 2026-07-01 01:24:48 UTC | 48.6s | `1.656` | `1.654` | $0.33 | $0.00 | $0.000000 | **-0.0004** | `-9.1%` | `STOP_LOSS_HIT` | $0.0704 |
| 6 | `SHORT` | 2026-07-01 02:37:59 UTC | 2026-07-01 02:38:07 UTC | 7.8s | `1.696` | `1.698` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0700 |
| 7 | `LONG` | 2026-07-01 02:58:59 UTC | 2026-07-01 02:59:47 UTC | 47.4s | `1.702` | `1.700` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0696 |
| 8 | `SHORT` | 2026-07-01 03:16:59 UTC | 2026-07-01 03:17:03 UTC | 3.8s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 9 | `LONG` | 2026-07-01 03:38:59 UTC | 2026-07-01 03:39:14 UTC | 14.8s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 10 | `SHORT` | 2026-07-01 04:00:59 UTC | 2026-07-01 04:01:30 UTC | 30.5s | `1.707` | `1.709` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0700 |
| 11 | `LONG` | 2026-07-01 04:20:59 UTC | 2026-07-01 04:21:32 UTC | 32.7s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0696 |
| 12 | `SHORT` | 2026-07-01 04:36:59 UTC | 2026-07-01 04:37:14 UTC | 14.7s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 13 | `LONG` | 2026-07-01 04:57:59 UTC | 2026-07-01 04:58:19 UTC | 19.2s | `1.703` | `1.701` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0696 |
| 14 | `SHORT` | 2026-07-01 05:22:59 UTC | 2026-07-01 05:26:59 UTC | 3m 59s | `1.701` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 15 | `LONG` | 2026-07-01 05:29:59 UTC | 2026-07-01 05:30:33 UTC | 33.0s | `1.707` | `1.705` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0696 |
| 16 | `SHORT` | 2026-07-01 05:32:59 UTC | 2026-07-01 05:37:20 UTC | 4m 20s | `1.702` | `1.700` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 17 | `LONG` | 2026-07-01 05:45:59 UTC | 2026-07-01 05:46:15 UTC | 15.3s | `1.706` | `1.704` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0696 |
| 18 | `SHORT` | 2026-07-01 06:03:59 UTC | 2026-07-01 06:04:15 UTC | 15.8s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0692 |
| 19 | `LONG` | 2026-07-01 06:14:59 UTC | 2026-07-01 06:15:20 UTC | 20.4s | `1.711` | `1.709` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0688 |
| 20 | `SHORT` | 2026-07-01 06:19:59 UTC | 2026-07-01 06:21:46 UTC | 1m 46s | `1.705` | `1.703` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 21 | `LONG` | 2026-07-01 06:54:59 UTC | 2026-07-01 06:56:00 UTC | 1m 00s | `1.692` | `1.690` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.9%` | `STOP_LOSS_HIT` | $0.0688 |
| 22 | `SHORT` | 2026-07-01 06:57:59 UTC | 2026-07-01 06:59:08 UTC | 1m 08s | `1.691` | `1.689` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 23 | `SHORT` | 2026-07-01 07:00:59 UTC | 2026-07-01 07:01:56 UTC | 56.8s | `1.692` | `1.690` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 24 | `SHORT` | 2026-07-01 07:04:59 UTC | 2026-07-01 07:05:24 UTC | 24.2s | `1.688` | `1.686` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 25 | `LONG` | 2026-07-01 07:13:59 UTC | 2026-07-01 07:14:30 UTC | 30.2s | `1.687` | `1.689` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| ... | ... | *(2365 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2391 | `LONG` | 2026-07-23 18:22:59 UTC | 2026-07-23 18:25:10 UTC | 2m 10s | `1.600` | `1.602` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.0656 |
| 2392 | `SHORT` | 2026-07-23 18:43:59 UTC | 2026-07-23 18:46:08 UTC | 2m 08s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0652 |
| 2393 | `LONG` | 2026-07-23 18:49:59 UTC | 2026-07-23 18:50:43 UTC | 43.8s | `1.609` | `1.607` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0648 |
| 2394 | `SHORT` | 2026-07-23 19:07:59 UTC | 2026-07-23 19:08:33 UTC | 33.7s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 2395 | `SHORT` | 2026-07-23 19:09:59 UTC | 2026-07-23 19:10:50 UTC | 50.6s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0656 |
| 2396 | `SHORT` | 2026-07-23 19:11:59 UTC | 2026-07-23 19:12:14 UTC | 14.3s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0652 |
| 2397 | `LONG` | 2026-07-23 19:13:59 UTC | 2026-07-23 19:15:07 UTC | 1m 07s | `1.609` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0656 |
| 2398 | `LONG` | 2026-07-23 19:16:59 UTC | 2026-07-23 19:18:59 UTC | 1m 59s | `1.612` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0652 |
| 2399 | `SHORT` | 2026-07-23 19:20:59 UTC | 2026-07-23 19:21:23 UTC | 23.5s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0648 |
| 2400 | `LONG` | 2026-07-23 19:22:59 UTC | 2026-07-23 19:23:49 UTC | 49.0s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 2401 | `SHORT` | 2026-07-23 19:39:59 UTC | 2026-07-23 19:40:04 UTC | 4.8s | `1.615` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0656 |
| 2402 | `LONG` | 2026-07-23 19:58:59 UTC | 2026-07-23 19:59:12 UTC | 12.5s | `1.615` | `1.617` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0660 |
| 2403 | `SHORT` | 2026-07-23 20:25:59 UTC | 2026-07-23 20:26:53 UTC | 53.5s | `1.621` | `1.623` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0656 |
| 2404 | `LONG` | 2026-07-23 20:31:59 UTC | 2026-07-23 20:33:41 UTC | 1m 41s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.2%` | `STOP_LOSS_HIT` | $0.0652 |
| 2405 | `LONG` | 2026-07-23 20:38:59 UTC | 2026-07-23 20:39:32 UTC | 32.4s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.2%` | `STOP_LOSS_HIT` | $0.0648 |
| 2406 | `SHORT` | 2026-07-23 20:40:59 UTC | 2026-07-23 20:50:54 UTC | 9m 54s | `1.619` | `1.621` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0644 |
| 2407 | `LONG` | 2026-07-23 20:53:59 UTC | 2026-07-23 20:55:28 UTC | 1m 28s | `1.621` | `1.623` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0648 |
| 2408 | `SHORT` | 2026-07-23 21:08:59 UTC | 2026-07-23 21:13:00 UTC | 4m 00s | `1.619` | `1.617` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 2409 | `LONG` | 2026-07-23 21:54:59 UTC | 2026-07-23 21:55:20 UTC | 20.1s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0656 |
| 2410 | `SHORT` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:24 UTC | 24.5s | `1.607` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0652 |
| 2411 | `LONG` | 2026-07-23 22:23:59 UTC | 2026-07-23 22:24:25 UTC | 25.1s | `1.615` | `1.617` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0656 |
| 2412 | `SHORT` | 2026-07-23 22:31:59 UTC | 2026-07-23 22:36:10 UTC | 4m 10s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0660 |
| 2413 | `LONG` | 2026-07-23 23:01:59 UTC | 2026-07-23 23:02:27 UTC | 27.6s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0664 |
| 2414 | `LONG` | 2026-07-23 23:17:59 UTC | 2026-07-23 23:22:40 UTC | 4m 40s | `1.606` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 2415 | `SHORT` | 2026-07-23 23:33:59 UTC | 2026-07-23 23:40:24 UTC | 6m 24s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0672 |

> 💡 *Full granular dataset with all 2415 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
