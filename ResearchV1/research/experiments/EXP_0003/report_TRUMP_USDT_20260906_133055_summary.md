# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:00:56 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.0964 USDT` | `₹9.10` | `+37.71%` |
| **Net Realized PnL** | **`+0.0264 USDT`** | **`₹+2.49`** | **`+37.71% Net ROI`** |
| **Gross Profit** | `+0.8160 USDT` | `₹77.07` | Total positive trade returns |
| **Gross Loss** | `-0.7896 USDT` | `₹74.58` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.03`** | — | Profitable |
| **Win / Loss Payoff** | `1.00` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0200 USDT` | `₹1.89` | **`-18.18%` Peak-to-Trough** |
| **Win Rate** | **`50.82%`** | — | `2040 Wins / 1974 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `1.60` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `1.60` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `2.07` | — | Net ROI divided by Max Drawdown |

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
| **Total Trades Executed** | `4014` | Total completed trade lifecycle events |
| **Winning Trades** | `2040` | `50.82%` of total trades |
| **Losing Trades** | `1974` | `49.18%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0004 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0004 USDT (-9.0% ROE)` | Trade #2 (SHORT) |
| **Max Consecutive Wins** | `10` trades | Peak winning streak |
| **Max Consecutive Losses** | `12` trades | Peak losing streak |
| **Average Trade Duration** | `1m 39s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #347 |
| **Longest Trade In-Position** | `23m 44s` | Trade #1937 |
| **Cumulative Time In Position** | `110h 32m 20s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1985` (49.5%) | `2029` (50.5%) | `4014` |
| **Wins / Losses** | `1021 W / 964 L` | `1019 W / 1010 L` | `2040 W / 1974 L` |
| **Win Rate** | **`51.44%`** | **`50.22%`** | **`50.82%`** |
| **Gross Profit** | `+0.4084 USDT` | `+0.4076 USDT` | `+0.8160 USDT` |
| **Gross Loss** | `-0.3856 USDT` | `-0.4040 USDT` | `-0.7896 USDT` |
| **Net Realized PnL** | **`+0.0228 USDT`** | **`+0.0036 USDT`** | **`+0.0264 USDT`** |
| **Net PnL (INR)** | `₹+2.15` | `₹+0.34` | `₹+2.49` |
| **Profit Factor** | `1.06` | `1.01` | `1.03` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `2040` | `50.8%` | `+0.8160 USDT` | `₹+77.07` | `100.0%` | `1m 38s` |
| `STOP_LOSS_HIT` | `1974` | `49.2%` | `-0.7896 USDT` | `₹-74.58` | `0.0%` | `1m 40s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:29:47 UTC | 47.6s | `1.661` | `1.663` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:38:28 UTC | 1m 28s | `1.664` | `1.666` | $0.33 | $0.00 | $0.000000 | **-0.0004** | `-9.0%` | `STOP_LOSS_HIT` | $0.0700 |
| 3 | `LONG` | 2026-07-01 00:41:59 UTC | 2026-07-01 00:46:07 UTC | 4m 07s | `1.665` | `1.667` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 4 | `SHORT` | 2026-07-01 00:55:59 UTC | 2026-07-01 00:56:42 UTC | 42.7s | `1.669` | `1.667` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 5 | `LONG` | 2026-07-01 01:01:59 UTC | 2026-07-01 01:02:09 UTC | 9.1s | `1.667` | `1.669` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 6 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:10:35 UTC | 35.3s | `1.661` | `1.659` | $0.33 | $0.00 | $0.000000 | **-0.0004** | `-9.0%` | `STOP_LOSS_HIT` | $0.0708 |
| 7 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:03 UTC | 3.2s | `1.645` | `1.647` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 8 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:23:12 UTC | 12.6s | `1.658` | `1.656` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0716 |
| 9 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:35:12 UTC | 12.7s | `1.658` | `1.660` | $0.33 | $0.00 | $0.000000 | **-0.0004** | `-9.0%` | `STOP_LOSS_HIT` | $0.0712 |
| 10 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:48:18 UTC | 18.9s | `1.676` | `1.678` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.9%` | `STOP_LOSS_HIT` | $0.0708 |
| 11 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:10 UTC | 10.2s | `1.676` | `1.678` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 12 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 01:59:04 UTC | 4.8s | `1.678` | `1.680` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.9%` | `STOP_LOSS_HIT` | $0.0708 |
| 13 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:04:23 UTC | 23.1s | `1.685` | `1.683` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.9%` | `STOP_LOSS_HIT` | $0.0704 |
| 14 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:09:39 UTC | 39.7s | `1.684` | `1.686` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 15 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:18:16 UTC | 17.0s | `1.702` | `1.704` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0704 |
| 16 | `LONG` | 2026-07-01 02:22:59 UTC | 2026-07-01 02:23:00 UTC | 0.9s | `1.709` | `1.707` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0700 |
| 17 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:13 UTC | 1m 13s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 18 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:05 UTC | 5.7s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 19 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:42:33 UTC | 1m 33s | `1.697` | `1.695` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0704 |
| 20 | `LONG` | 2026-07-01 02:44:59 UTC | 2026-07-01 02:45:29 UTC | 29.3s | `1.700` | `1.698` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0700 |
| 21 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:24 UTC | 24.7s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0696 |
| 22 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:05 UTC | 5.9s | `1.707` | `1.709` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0692 |
| 23 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:04 UTC | 4.8s | `1.729` | `1.727` | $0.35 | $0.00 | $0.000000 | **+0.0004** | `+8.7%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 24 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:00 UTC | 0.7s | `1.711` | `1.709` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0692 |
| 25 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:20:09 UTC | 9.5s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **-0.0004** | `-8.8%` | `STOP_LOSS_HIT` | $0.0688 |
| ... | ... | *(3964 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 3990 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 20:33:41 UTC | 5m 41s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.2%` | `STOP_LOSS_HIT` | $0.0980 |
| 3991 | `LONG` | 2026-07-23 20:45:59 UTC | 2026-07-23 20:46:24 UTC | 24.0s | `1.618` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0984 |
| 3992 | `SHORT` | 2026-07-23 20:52:59 UTC | 2026-07-23 20:55:28 UTC | 2m 28s | `1.621` | `1.623` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0980 |
| 3993 | `SHORT` | 2026-07-23 20:57:59 UTC | 2026-07-23 21:01:39 UTC | 3m 39s | `1.623` | `1.625` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.2%` | `STOP_LOSS_HIT` | $0.0976 |
| 3994 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:07:45 UTC | 1m 45s | `1.622` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.0980 |
| 3995 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:18:00 UTC | 0.4s | `1.617` | `1.615` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0976 |
| 3996 | `LONG` | 2026-07-23 21:22:59 UTC | 2026-07-23 21:23:03 UTC | 4.0s | `1.614` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0972 |
| 3997 | `SHORT` | 2026-07-23 21:30:59 UTC | 2026-07-23 21:32:14 UTC | 1m 14s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0976 |
| 3998 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:38:00 UTC | 0.2s | `1.603` | `1.601` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.4%` | `STOP_LOSS_HIT` | $0.0972 |
| 3999 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 21:46:15 UTC | 15.1s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0968 |
| 4000 | `SHORT` | 2026-07-23 21:48:59 UTC | 2026-07-23 21:49:21 UTC | 21.1s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0964 |
| 4001 | `SHORT` | 2026-07-23 22:00:59 UTC | 2026-07-23 22:02:05 UTC | 1m 05s | `1.609` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0968 |
| 4002 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:12:34 UTC | 34.5s | `1.611` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0964 |
| 4003 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:24 UTC | 24.5s | `1.607` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0968 |
| 4004 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:20 UTC | 20.1s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0972 |
| 4005 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0976 |
| 4006 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:36:10 UTC | 1m 10s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0972 |
| 4007 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:41:36 UTC | 37.0s | `1.604` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.0976 |
| 4008 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 22:55:31 UTC | 5m 31s | `1.607` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0972 |
| 4009 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:10:04 UTC | 1m 04s | `1.605` | `1.603` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0968 |
| 4010 | `SHORT` | 2026-07-23 23:19:59 UTC | 2026-07-23 23:22:40 UTC | 2m 40s | `1.606` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0964 |
| 4011 | `SHORT` | 2026-07-23 23:24:59 UTC | 2026-07-23 23:25:35 UTC | 35.3s | `1.607` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.3%` | `STOP_LOSS_HIT` | $0.0960 |
| 4012 | `SHORT` | 2026-07-23 23:29:59 UTC | 2026-07-23 23:31:48 UTC | 1m 48s | `1.608` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0964 |
| 4013 | `LONG` | 2026-07-23 23:36:59 UTC | 2026-07-23 23:39:12 UTC | 2m 12s | `1.606` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.0968 |
| 4014 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-23 23:56:26 UTC | 1m 26s | `1.599` | `1.597` | $0.32 | $0.00 | $0.000000 | **-0.0004** | `-9.4%` | `STOP_LOSS_HIT` | $0.0964 |

> 💡 *Full granular dataset with all 4014 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
