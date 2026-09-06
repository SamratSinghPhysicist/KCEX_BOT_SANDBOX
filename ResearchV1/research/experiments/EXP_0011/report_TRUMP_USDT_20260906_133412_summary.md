# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:04:12 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.2452 USDT` | `₹23.16` | `+250.29%` |
| **Net Realized PnL** | **`+0.1752 USDT`** | **`₹+16.55`** | **`+250.29% Net ROI`** |
| **Gross Profit** | `+0.8280 USDT` | `₹78.20` | Total positive trade returns |
| **Gross Loss** | `-0.6528 USDT` | `₹61.66` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.27`** | — | Profitable |
| **Win / Loss Payoff** | `0.22` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0208 USDT` | `₹1.96` | **`-13.39%` Peak-to-Trough** |
| **Win Rate** | **`85.47%`** | — | `2070 Wins / 352 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `7.58` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `3.26` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `18.69` | — | Net ROI divided by Max Drawdown |

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
| **Stop Loss Rule** | `-12 ticks away from entry (0.012 USDT)` | Stop loss evaluation logic |

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
| **Total Trades Executed** | `2422` | Total completed trade lifecycle events |
| **Winning Trades** | `2070` | `85.47%` of total trades |
| **Losing Trades** | `352` | `14.53%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0001 USDT` (`₹+0.01`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0019 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0024 USDT (-49.6% ROE)` | Trade #453 (SHORT) |
| **Max Consecutive Wins** | `49` trades | Peak winning streak |
| **Max Consecutive Losses** | `4` trades | Peak losing streak |
| **Average Trade Duration** | `7m 40s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #1494 |
| **Longest Trade In-Position** | `2h 22m 33s` | Trade #1372 |
| **Cumulative Time In Position** | `309h 49m 06s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1205` (49.8%) | `1217` (50.2%) | `2422` |
| **Wins / Losses** | `1020 W / 185 L` | `1050 W / 167 L` | `2070 W / 352 L` |
| **Win Rate** | **`84.65%`** | **`86.28%`** | **`85.47%`** |
| **Gross Profit** | `+0.4080 USDT` | `+0.4200 USDT` | `+0.8280 USDT` |
| **Gross Loss** | `-0.3438 USDT` | `-0.3090 USDT` | `-0.6528 USDT` |
| **Net Realized PnL** | **`+0.0642 USDT`** | **`+0.1110 USDT`** | **`+0.1752 USDT`** |
| **Net PnL (INR)** | `₹+6.06` | `₹+10.48` | `₹+16.55` |
| **Profit Factor** | `1.19` | `1.36` | `1.27` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `2070` | `85.5%` | `+0.8280 USDT` | `₹+78.20` | `100.0%` | `5m 30s` |
| `STOP_LOSS_HIT` | `352` | `14.5%` | `-0.6528 USDT` | `₹-61.66` | `0.0%` | `20m 22s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:29:47 UTC | 47.6s | `1.661` | `1.663` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 01:05:16 UTC | 28m 16s | `1.664` | `1.662` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 3 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:12:44 UTC | 2m 44s | `1.661` | `1.652` | $0.33 | $0.00 | $0.000000 | **-0.0018** | `-40.6%` | `STOP_LOSS_HIT` | $0.0690 |
| 4 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:03 UTC | 3.2s | `1.645` | `1.647` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0694 |
| 5 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:23:12 UTC | 12.6s | `1.658` | `1.656` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0698 |
| 6 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:38:46 UTC | 3m 46s | `1.658` | `1.667` | $0.33 | $0.00 | $0.000000 | **-0.0018** | `-40.7%` | `STOP_LOSS_HIT` | $0.0680 |
| 7 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:09 UTC | 2m 09s | `1.676` | `1.674` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 8 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:10 UTC | 10.2s | `1.676` | `1.678` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 9 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:03:45 UTC | 4m 45s | `1.678` | `1.687` | $0.34 | $0.00 | $0.000000 | **-0.0018** | `-40.2%` | `STOP_LOSS_HIT` | $0.0670 |
| 10 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:09:39 UTC | 39.7s | `1.684` | `1.686` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0674 |
| 11 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:37:07 UTC | 19m 07s | `1.702` | `1.700` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0678 |
| 12 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:01 UTC | 3m 01s | `1.697` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0682 |
| 13 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:05:28 UTC | 4m 28s | `1.704` | `1.714` | $0.34 | $0.00 | $0.000000 | **-0.0020** | `-44.0%` | `STOP_LOSS_HIT` | $0.0662 |
| 14 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:04 UTC | 4.8s | `1.729` | `1.727` | $0.35 | $0.00 | $0.000000 | **+0.0004** | `+8.7%` | `MIN_PROFIT_TP_HIT` | $0.0666 |
| 15 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:17:39 UTC | 1m 39s | `1.711` | `1.701` | $0.34 | $0.00 | $0.000000 | **-0.0020** | `-43.8%` | `STOP_LOSS_HIT` | $0.0646 |
| 16 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:37:08 UTC | 17m 08s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0650 |
| 17 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:48:40 UTC | 6m 40s | `1.706` | `1.704` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0654 |
| 18 | `LONG` | 2026-07-01 03:51:59 UTC | 2026-07-01 03:52:16 UTC | 16.2s | `1.711` | `1.713` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0658 |
| 19 | `SHORT` | 2026-07-01 03:56:59 UTC | 2026-07-01 03:57:03 UTC | 3.5s | `1.712` | `1.710` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0662 |
| 20 | `LONG` | 2026-07-01 04:02:59 UTC | 2026-07-01 04:04:04 UTC | 1m 04s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0666 |
| 21 | `LONG` | 2026-07-01 04:11:59 UTC | 2026-07-01 04:16:02 UTC | 4m 02s | `1.700` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0670 |
| 22 | `SHORT` | 2026-07-01 04:21:59 UTC | 2026-07-01 04:23:55 UTC | 1m 55s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0674 |
| 23 | `LONG` | 2026-07-01 04:27:59 UTC | 2026-07-01 04:31:23 UTC | 3m 23s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0678 |
| 24 | `LONG` | 2026-07-01 04:38:59 UTC | 2026-07-01 04:41:01 UTC | 2m 01s | `1.700` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0682 |
| 25 | `SHORT` | 2026-07-01 04:59:59 UTC | 2026-07-01 05:00:10 UTC | 10.4s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0686 |
| ... | ... | *(2372 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2398 | `LONG` | 2026-07-23 17:04:59 UTC | 2026-07-23 17:40:48 UTC | 35m 48s | `1.621` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0018** | `-41.6%` | `STOP_LOSS_HIT` | $0.2488 |
| 2399 | `SHORT` | 2026-07-23 17:47:59 UTC | 2026-07-23 17:53:13 UTC | 5m 13s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2492 |
| 2400 | `LONG` | 2026-07-23 18:02:59 UTC | 2026-07-23 18:11:14 UTC | 8m 14s | `1.599` | `1.590` | $0.32 | $0.00 | $0.000000 | **-0.0018** | `-42.2%` | `STOP_LOSS_HIT` | $0.2474 |
| 2401 | `SHORT` | 2026-07-23 18:12:59 UTC | 2026-07-23 18:16:12 UTC | 3m 12s | `1.594` | `1.592` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2478 |
| 2402 | `SHORT` | 2026-07-23 18:17:59 UTC | 2026-07-23 18:18:03 UTC | 3.1s | `1.589` | `1.587` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2482 |
| 2403 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:30:28 UTC | 1m 28s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2486 |
| 2404 | `LONG` | 2026-07-23 18:35:59 UTC | 2026-07-23 19:02:40 UTC | 26m 40s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2490 |
| 2405 | `SHORT` | 2026-07-23 19:06:59 UTC | 2026-07-23 19:25:52 UTC | 18m 52s | `1.609` | `1.618` | $0.32 | $0.00 | $0.000000 | **-0.0018** | `-42.0%` | `STOP_LOSS_HIT` | $0.2472 |
| 2406 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:29:04 UTC | 4.2s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2476 |
| 2407 | `LONG` | 2026-07-23 19:40:59 UTC | 2026-07-23 19:58:16 UTC | 17m 16s | `1.613` | `1.615` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2480 |
| 2408 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2484 |
| 2409 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 21:01:39 UTC | 33m 39s | `1.623` | `1.625` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2488 |
| 2410 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:07:45 UTC | 1m 45s | `1.622` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2492 |
| 2411 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:32:14 UTC | 14m 14s | `1.617` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0018** | `-41.7%` | `STOP_LOSS_HIT` | $0.2474 |
| 2412 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:38:30 UTC | 30.0s | `1.603` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2478 |
| 2413 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 22:06:32 UTC | 20m 32s | `1.605` | `1.614` | $0.32 | $0.00 | $0.000000 | **-0.0018** | `-42.1%` | `STOP_LOSS_HIT` | $0.2460 |
| 2414 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:17 UTC | 5m 17s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2464 |
| 2415 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:24 UTC | 24.5s | `1.607` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2468 |
| 2416 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:20 UTC | 20.1s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2472 |
| 2417 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2476 |
| 2418 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:40:01 UTC | 5m 01s | `1.611` | `1.602` | $0.32 | $0.00 | $0.000000 | **-0.0018** | `-41.9%` | `STOP_LOSS_HIT` | $0.2458 |
| 2419 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:35 UTC | 11m 35s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2462 |
| 2420 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:16:13 UTC | 7m 13s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2466 |
| 2421 | `SHORT` | 2026-07-23 23:19:59 UTC | 2026-07-23 23:47:35 UTC | 27m 35s | `1.606` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2470 |
| 2422 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:07:16 UTC | 12m 16s | `1.599` | `1.590` | $0.32 | $0.00 | $0.000000 | **-0.0018** | `-42.2%` | `STOP_LOSS_HIT` | $0.2452 |

> 💡 *Full granular dataset with all 2422 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
