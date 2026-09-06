# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:02:32 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.1896 USDT` | `₹17.91` | `+170.86%` |
| **Net Realized PnL** | **`+0.1196 USDT`** | **`₹+11.30`** | **`+170.86% Net ROI`** |
| **Gross Profit** | `+0.9284 USDT` | `₹87.69` | Total positive trade returns |
| **Gross Loss** | `-0.8088 USDT` | `₹76.39` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.15`** | — | Profitable |
| **Win / Loss Payoff** | `0.67` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0116 USDT` | `₹1.10` | **`-15.30%` Peak-to-Trough** |
| **Win Rate** | **`63.26%`** | — | `2321 Wins / 1348 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `5.21` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `4.20` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `11.16` | — | Net ROI divided by Max Drawdown |

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
| **Stop Loss Rule** | `-3 ticks away from entry (0.003 USDT)` | Stop loss evaluation logic |

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
| **Total Trades Executed** | `3669` | Total completed trade lifecycle events |
| **Winning Trades** | `2321` | `63.26%` of total trades |
| **Losing Trades** | `1348` | `36.74%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0006 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0006 USDT (-13.5% ROE)` | Trade #2 (SHORT) |
| **Max Consecutive Wins** | `17` trades | Peak winning streak |
| **Max Consecutive Losses** | `8` trades | Peak losing streak |
| **Average Trade Duration** | `2m 42s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #328 |
| **Longest Trade In-Position** | `43m 20s` | Trade #2688 |
| **Cumulative Time In Position** | `165h 29m 37s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1802` (49.1%) | `1867` (50.9%) | `3669` |
| **Wins / Losses** | `1150 W / 652 L` | `1171 W / 696 L` | `2321 W / 1348 L` |
| **Win Rate** | **`63.82%`** | **`62.72%`** | **`63.26%`** |
| **Gross Profit** | `+0.4600 USDT` | `+0.4684 USDT` | `+0.9284 USDT` |
| **Gross Loss** | `-0.3912 USDT` | `-0.4176 USDT` | `-0.8088 USDT` |
| **Net Realized PnL** | **`+0.0688 USDT`** | **`+0.0508 USDT`** | **`+0.1196 USDT`** |
| **Net PnL (INR)** | `₹+6.50` | `₹+4.80` | `₹+11.30` |
| **Profit Factor** | `1.18` | `1.12` | `1.15` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `2321` | `63.3%` | `+0.9284 USDT` | `₹+87.69` | `100.0%` | `2m 22s` |
| `STOP_LOSS_HIT` | `1348` | `36.7%` | `-0.8088 USDT` | `₹-76.39` | `0.0%` | `3m 16s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:29:47 UTC | 47.6s | `1.661` | `1.663` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:46:07 UTC | 9m 07s | `1.664` | `1.667` | $0.33 | $0.00 | $0.000000 | **-0.0006** | `-13.5%` | `STOP_LOSS_HIT` | $0.0698 |
| 3 | `SHORT` | 2026-07-01 00:55:59 UTC | 2026-07-01 00:56:42 UTC | 42.7s | `1.669` | `1.667` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0702 |
| 4 | `LONG` | 2026-07-01 01:01:59 UTC | 2026-07-01 01:02:09 UTC | 9.1s | `1.667` | `1.669` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 5 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:10:40 UTC | 40.7s | `1.661` | `1.658` | $0.33 | $0.00 | $0.000000 | **-0.0006** | `-13.5%` | `STOP_LOSS_HIT` | $0.0700 |
| 6 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:03 UTC | 3.2s | `1.645` | `1.647` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 7 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:23:12 UTC | 12.6s | `1.658` | `1.656` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 8 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:35:33 UTC | 33.8s | `1.658` | `1.661` | $0.33 | $0.00 | $0.000000 | **-0.0006** | `-13.6%` | `STOP_LOSS_HIT` | $0.0702 |
| 9 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:09 UTC | 2m 09s | `1.676` | `1.674` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 10 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:10 UTC | 10.2s | `1.676` | `1.678` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0710 |
| 11 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:01:16 UTC | 2m 16s | `1.678` | `1.681` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.4%` | `STOP_LOSS_HIT` | $0.0704 |
| 12 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:04:36 UTC | 36.0s | `1.685` | `1.682` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.4%` | `STOP_LOSS_HIT` | $0.0698 |
| 13 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:09:39 UTC | 39.7s | `1.684` | `1.686` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0702 |
| 14 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:18:17 UTC | 17.5s | `1.702` | `1.705` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.2%` | `STOP_LOSS_HIT` | $0.0696 |
| 15 | `LONG` | 2026-07-01 02:22:59 UTC | 2026-07-01 02:23:00 UTC | 0.9s | `1.709` | `1.706` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.2%` | `STOP_LOSS_HIT` | $0.0690 |
| 16 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:13 UTC | 1m 13s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0694 |
| 17 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:05 UTC | 5.7s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0698 |
| 18 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:01 UTC | 3m 01s | `1.697` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0702 |
| 19 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:33 UTC | 33.3s | `1.704` | `1.707` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.2%` | `STOP_LOSS_HIT` | $0.0696 |
| 20 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:07 UTC | 7.4s | `1.707` | `1.710` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.2%` | `STOP_LOSS_HIT` | $0.0690 |
| 21 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:04 UTC | 4.8s | `1.729` | `1.727` | $0.35 | $0.00 | $0.000000 | **+0.0004** | `+8.7%` | `MIN_PROFIT_TP_HIT` | $0.0694 |
| 22 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:00 UTC | 0.7s | `1.711` | `1.708` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.2%` | `STOP_LOSS_HIT` | $0.0688 |
| 23 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:20:11 UTC | 11.2s | `1.704` | `1.701` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.2%` | `STOP_LOSS_HIT` | $0.0682 |
| 24 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:29:01 UTC | 1m 01s | `1.699` | `1.701` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0686 |
| 25 | `SHORT` | 2026-07-01 03:32:59 UTC | 2026-07-01 03:34:17 UTC | 1m 17s | `1.699` | `1.697` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0690 |
| ... | ... | *(3619 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 3645 | `LONG` | 2026-07-23 19:52:59 UTC | 2026-07-23 19:54:09 UTC | 1m 09s | `1.609` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1890 |
| 3646 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1894 |
| 3647 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 20:33:41 UTC | 5m 41s | `1.623` | `1.620` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-13.9%` | `STOP_LOSS_HIT` | $0.1888 |
| 3648 | `LONG` | 2026-07-23 20:45:59 UTC | 2026-07-23 20:46:24 UTC | 24.0s | `1.618` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1892 |
| 3649 | `SHORT` | 2026-07-23 20:52:59 UTC | 2026-07-23 20:57:43 UTC | 4m 43s | `1.621` | `1.624` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-13.9%` | `STOP_LOSS_HIT` | $0.1886 |
| 3650 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:07:45 UTC | 1m 45s | `1.622` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.1890 |
| 3651 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:18:08 UTC | 8.4s | `1.617` | `1.614` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-13.9%` | `STOP_LOSS_HIT` | $0.1884 |
| 3652 | `LONG` | 2026-07-23 21:22:59 UTC | 2026-07-23 21:29:06 UTC | 6m 06s | `1.614` | `1.611` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-13.9%` | `STOP_LOSS_HIT` | $0.1878 |
| 3653 | `SHORT` | 2026-07-23 21:30:59 UTC | 2026-07-23 21:32:14 UTC | 1m 14s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1882 |
| 3654 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:38:30 UTC | 30.0s | `1.603` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.1886 |
| 3655 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 21:46:26 UTC | 26.3s | `1.605` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-14.0%` | `STOP_LOSS_HIT` | $0.1880 |
| 3656 | `SHORT` | 2026-07-23 21:48:59 UTC | 2026-07-23 21:55:30 UTC | 6m 30s | `1.605` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-14.0%` | `STOP_LOSS_HIT` | $0.1874 |
| 3657 | `SHORT` | 2026-07-23 22:00:59 UTC | 2026-07-23 22:02:05 UTC | 1m 05s | `1.609` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1878 |
| 3658 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:17 UTC | 5m 17s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1882 |
| 3659 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:24 UTC | 24.5s | `1.607` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1886 |
| 3660 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:20 UTC | 20.1s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1890 |
| 3661 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1894 |
| 3662 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:37:16 UTC | 2m 16s | `1.611` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-14.0%` | `STOP_LOSS_HIT` | $0.1888 |
| 3663 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:41:36 UTC | 37.0s | `1.604` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.1892 |
| 3664 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:35 UTC | 11m 35s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1896 |
| 3665 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:16:13 UTC | 7m 13s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1900 |
| 3666 | `SHORT` | 2026-07-23 23:19:59 UTC | 2026-07-23 23:25:35 UTC | 5m 35s | `1.606` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-14.0%` | `STOP_LOSS_HIT` | $0.1894 |
| 3667 | `SHORT` | 2026-07-23 23:29:59 UTC | 2026-07-23 23:31:48 UTC | 1m 48s | `1.608` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1898 |
| 3668 | `LONG` | 2026-07-23 23:36:59 UTC | 2026-07-23 23:39:12 UTC | 2m 12s | `1.606` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.1902 |
| 3669 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:03:59 UTC | 8m 59s | `1.599` | `1.596` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-14.1%` | `STOP_LOSS_HIT` | $0.1896 |

> 💡 *Full granular dataset with all 3669 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
