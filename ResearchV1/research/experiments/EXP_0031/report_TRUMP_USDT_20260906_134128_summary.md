# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:11:28 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.1084 USDT` | `₹10.24` | `+54.86%` |
| **Net Realized PnL** | **`+0.0384 USDT`** | **`₹+3.63`** | **`+54.86% Net ROI`** |
| **Gross Profit** | `+0.9912 USDT` | `₹93.62` | Total positive trade returns |
| **Gross Loss** | `-0.9528 USDT` | `₹89.99` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.04`** | — | Profitable |
| **Win / Loss Payoff** | `1.00` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0536 USDT` | `₹5.06` | **`-38.40%` Peak-to-Trough** |
| **Win Rate** | **`50.99%`** | — | `1239 Wins / 1191 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `1.86` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `1.87` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `1.43` | — | Net ROI divided by Max Drawdown |

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
| **Take Profit Target** | `+4 ticks` (`+0.004 USDT`) | Guaranteed Min-Profit TP (`entry + N*pu`) |
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
| **Total Trades Executed** | `2430` | Total completed trade lifecycle events |
| **Winning Trades** | `1239` | `50.99%` of total trades |
| **Losing Trades** | `1191` | `49.01%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0008 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0008 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0008 USDT (+18.1% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0008 USDT (-18.0% ROE)` | Trade #2 (SHORT) |
| **Max Consecutive Wins** | `9` trades | Peak winning streak |
| **Max Consecutive Losses** | `11` trades | Peak losing streak |
| **Average Trade Duration** | `7m 53s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.8s` | Trade #509 |
| **Longest Trade In-Position** | `1h 58m 09s` | Trade #1364 |
| **Cumulative Time In Position** | `319h 38m 29s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1193` (49.1%) | `1237` (50.9%) | `2430` |
| **Wins / Losses** | `612 W / 581 L` | `627 W / 610 L` | `1239 W / 1191 L` |
| **Win Rate** | **`51.30%`** | **`50.69%`** | **`50.99%`** |
| **Gross Profit** | `+0.4896 USDT` | `+0.5016 USDT` | `+0.9912 USDT` |
| **Gross Loss** | `-0.4648 USDT` | `-0.4880 USDT` | `-0.9528 USDT` |
| **Net Realized PnL** | **`+0.0248 USDT`** | **`+0.0136 USDT`** | **`+0.0384 USDT`** |
| **Net PnL (INR)** | `₹+2.34` | `₹+1.28` | `₹+3.63` |
| **Profit Factor** | `1.05` | `1.03` | `1.04` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1239` | `51.0%` | `+0.9912 USDT` | `₹+93.62` | `100.0%` | `7m 42s` |
| `STOP_LOSS_HIT` | `1191` | `49.0%` | `-0.9528 USDT` | `₹-89.99` | `0.0%` | `8m 04s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:30:53 UTC | 1m 53s | `1.661` | `1.665` | $0.33 | $0.00 | $0.000000 | **+0.0008** | `+18.1%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:52:00 UTC | 15m 00s | `1.664` | `1.668` | $0.33 | $0.00 | $0.000000 | **-0.0008** | `-18.0%` | `STOP_LOSS_HIT` | $0.0700 |
| 3 | `SHORT` | 2026-07-01 00:55:59 UTC | 2026-07-01 00:58:49 UTC | 2m 49s | `1.669` | `1.665` | $0.33 | $0.00 | $0.000000 | **+0.0008** | `+18.0%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 4 | `LONG` | 2026-07-01 01:01:59 UTC | 2026-07-01 01:05:02 UTC | 3m 02s | `1.667` | `1.663` | $0.33 | $0.00 | $0.000000 | **-0.0008** | `-18.0%` | `STOP_LOSS_HIT` | $0.0700 |
| 5 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:10:57 UTC | 57.2s | `1.661` | `1.657` | $0.33 | $0.00 | $0.000000 | **-0.0008** | `-18.1%` | `STOP_LOSS_HIT` | $0.0692 |
| 6 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:07 UTC | 7.5s | `1.645` | `1.649` | $0.33 | $0.00 | $0.000000 | **+0.0008** | `+18.2%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 7 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:24:48 UTC | 1m 48s | `1.658` | `1.654` | $0.33 | $0.00 | $0.000000 | **+0.0008** | `+18.1%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 8 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:35:43 UTC | 43.4s | `1.658` | `1.662` | $0.33 | $0.00 | $0.000000 | **-0.0008** | `-18.1%` | `STOP_LOSS_HIT` | $0.0700 |
| 9 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:54:41 UTC | 6m 41s | `1.676` | `1.680` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.9%` | `STOP_LOSS_HIT` | $0.0692 |
| 10 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:02:30 UTC | 3m 30s | `1.678` | `1.682` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.9%` | `STOP_LOSS_HIT` | $0.0684 |
| 11 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:04:58 UTC | 58.3s | `1.685` | `1.681` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.8%` | `STOP_LOSS_HIT` | $0.0676 |
| 12 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:10:07 UTC | 1m 07s | `1.684` | `1.688` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.8%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 13 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:18:18 UTC | 18.2s | `1.702` | `1.706` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0676 |
| 14 | `LONG` | 2026-07-01 02:22:59 UTC | 2026-07-01 02:23:00 UTC | 0.9s | `1.709` | `1.705` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0668 |
| 15 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:16 UTC | 1m 16s | `1.705` | `1.709` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.6%` | `MIN_PROFIT_TP_HIT` | $0.0676 |
| 16 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:46 UTC | 46.0s | `1.704` | `1.708` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.6%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 17 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:18 UTC | 3m 18s | `1.697` | `1.701` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.7%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 18 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:33 UTC | 33.3s | `1.704` | `1.708` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0684 |
| 19 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:07 UTC | 7.4s | `1.707` | `1.711` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0676 |
| 20 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:11 UTC | 11.4s | `1.729` | `1.725` | $0.35 | $0.00 | $0.000000 | **+0.0008** | `+17.4%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 21 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:12 UTC | 12.1s | `1.711` | `1.707` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.5%` | `STOP_LOSS_HIT` | $0.0676 |
| 22 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:20:21 UTC | 21.5s | `1.704` | `1.700` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0668 |
| 23 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:36:36 UTC | 8m 36s | `1.699` | `1.703` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.7%` | `MIN_PROFIT_TP_HIT` | $0.0676 |
| 24 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:46:48 UTC | 4m 48s | `1.706` | `1.710` | $0.34 | $0.00 | $0.000000 | **-0.0008** | `-17.6%` | `STOP_LOSS_HIT` | $0.0668 |
| 25 | `LONG` | 2026-07-01 03:51:59 UTC | 2026-07-01 03:52:23 UTC | 23.6s | `1.711` | `1.715` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.5%` | `MIN_PROFIT_TP_HIT` | $0.0676 |
| ... | ... | *(2380 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2406 | `LONG` | 2026-07-23 18:46:59 UTC | 2026-07-23 18:49:06 UTC | 2m 06s | `1.606` | `1.610` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1052 |
| 2407 | `SHORT` | 2026-07-23 18:51:59 UTC | 2026-07-23 19:02:40 UTC | 10m 40s | `1.608` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.7%` | `STOP_LOSS_HIT` | $0.1044 |
| 2408 | `SHORT` | 2026-07-23 19:06:59 UTC | 2026-07-23 19:12:14 UTC | 5m 14s | `1.609` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.1036 |
| 2409 | `LONG` | 2026-07-23 19:16:59 UTC | 2026-07-23 19:19:32 UTC | 2m 32s | `1.612` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.1028 |
| 2410 | `LONG` | 2026-07-23 19:22:59 UTC | 2026-07-23 19:25:50 UTC | 2m 50s | `1.610` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.1036 |
| 2411 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:41:22 UTC | 12m 22s | `1.616` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.1044 |
| 2412 | `LONG` | 2026-07-23 19:45:59 UTC | 2026-07-23 19:50:07 UTC | 4m 07s | `1.612` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.1036 |
| 2413 | `LONG` | 2026-07-23 19:52:59 UTC | 2026-07-23 19:57:45 UTC | 4m 45s | `1.609` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.1044 |
| 2414 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:40:29 UTC | 29m 29s | `1.623` | `1.619` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.5%` | `MIN_PROFIT_TP_HIT` | $0.1052 |
| 2415 | `LONG` | 2026-07-23 20:45:59 UTC | 2026-07-23 20:54:24 UTC | 8m 24s | `1.618` | `1.622` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.5%` | `MIN_PROFIT_TP_HIT` | $0.1060 |
| 2416 | `SHORT` | 2026-07-23 20:57:59 UTC | 2026-07-23 21:08:20 UTC | 10m 20s | `1.623` | `1.619` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.5%` | `MIN_PROFIT_TP_HIT` | $0.1068 |
| 2417 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:18:08 UTC | 8.4s | `1.617` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.1060 |
| 2418 | `LONG` | 2026-07-23 21:22:59 UTC | 2026-07-23 21:30:11 UTC | 7m 11s | `1.614` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.1052 |
| 2419 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:46:15 UTC | 8m 15s | `1.603` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1060 |
| 2420 | `SHORT` | 2026-07-23 21:48:59 UTC | 2026-07-23 21:55:50 UTC | 6m 50s | `1.605` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.7%` | `STOP_LOSS_HIT` | $0.1052 |
| 2421 | `SHORT` | 2026-07-23 22:00:59 UTC | 2026-07-23 22:06:10 UTC | 5m 10s | `1.609` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.1044 |
| 2422 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:55 UTC | 5m 55s | `1.611` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.1052 |
| 2423 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:20:50 UTC | 1m 50s | `1.607` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1060 |
| 2424 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:30:35 UTC | 2m 35s | `1.616` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.1068 |
| 2425 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:37:30 UTC | 2m 30s | `1.611` | `1.607` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.6%` | `STOP_LOSS_HIT` | $0.1060 |
| 2426 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:44:34 UTC | 3m 34s | `1.604` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1068 |
| 2427 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:04:35 UTC | 14m 35s | `1.607` | `1.603` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1076 |
| 2428 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:25:35 UTC | 16m 35s | `1.605` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1084 |
| 2429 | `SHORT` | 2026-07-23 23:29:59 UTC | 2026-07-23 23:47:35 UTC | 17m 35s | `1.608` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1092 |
| 2430 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:03:59 UTC | 8m 59s | `1.599` | `1.595` | $0.32 | $0.00 | $0.000000 | **-0.0008** | `-18.8%` | `STOP_LOSS_HIT` | $0.1084 |

> 💡 *Full granular dataset with all 2430 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
