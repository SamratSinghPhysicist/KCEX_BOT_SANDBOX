# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:10:26 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.1348 USDT` | `₹12.73` | `+92.57%` |
| **Net Realized PnL** | **`+0.0648 USDT`** | **`₹+6.12`** | **`+92.57% Net ROI`** |
| **Gross Profit** | `+0.9972 USDT` | `₹94.19` | Total positive trade returns |
| **Gross Loss** | `-0.9324 USDT` | `₹88.07` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.07`** | — | Profitable |
| **Win / Loss Payoff** | `1.00` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0186 USDT` | `₹1.76` | **`-15.75%` Peak-to-Trough** |
| **Win Rate** | **`51.68%`** | — | `1662 Wins / 1554 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `2.79` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `2.80` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `5.88` | — | Net ROI divided by Max Drawdown |

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
| **Take Profit Target** | `+3 ticks` (`+0.003 USDT`) | Guaranteed Min-Profit TP (`entry + N*pu`) |
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
| **Total Trades Executed** | `3216` | Total completed trade lifecycle events |
| **Winning Trades** | `1662` | `51.68%` of total trades |
| **Losing Trades** | `1554` | `48.32%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0006 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0006 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0006 USDT (+13.5% ROE)` | Trade #3 (SHORT) |
| **Largest Losing Trade** | `-0.0006 USDT (-13.5% ROE)` | Trade #2 (SHORT) |
| **Max Consecutive Wins** | `13` trades | Peak winning streak |
| **Max Consecutive Losses** | `11` trades | Peak losing streak |
| **Average Trade Duration** | `4m 15s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #304 |
| **Longest Trade In-Position** | `1h 07m 41s` | Trade #1788 |
| **Cumulative Time In Position** | `228h 21m 00s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1577` (49.0%) | `1639` (51.0%) | `3216` |
| **Wins / Losses** | `834 W / 743 L` | `828 W / 811 L` | `1662 W / 1554 L` |
| **Win Rate** | **`52.89%`** | **`50.52%`** | **`51.68%`** |
| **Gross Profit** | `+0.5004 USDT` | `+0.4968 USDT` | `+0.9972 USDT` |
| **Gross Loss** | `-0.4458 USDT` | `-0.4866 USDT` | `-0.9324 USDT` |
| **Net Realized PnL** | **`+0.0546 USDT`** | **`+0.0102 USDT`** | **`+0.0648 USDT`** |
| **Net PnL (INR)** | `₹+5.16` | `₹+0.96` | `₹+6.12` |
| **Profit Factor** | `1.12` | `1.02` | `1.07` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1662` | `51.7%` | `+0.9972 USDT` | `₹+94.19` | `100.0%` | `4m 14s` |
| `STOP_LOSS_HIT` | `1554` | `48.3%` | `-0.9324 USDT` | `₹-88.07` | `0.0%` | `4m 16s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:30:42 UTC | 1m 42s | `1.661` | `1.664` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.5%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:46:07 UTC | 9m 07s | `1.664` | `1.667` | $0.33 | $0.00 | $0.000000 | **-0.0006** | `-13.5%` | `STOP_LOSS_HIT` | $0.0700 |
| 3 | `SHORT` | 2026-07-01 00:55:59 UTC | 2026-07-01 00:56:42 UTC | 42.7s | `1.669` | `1.666` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.5%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 4 | `LONG` | 2026-07-01 01:01:59 UTC | 2026-07-01 01:04:18 UTC | 2m 18s | `1.667` | `1.664` | $0.33 | $0.00 | $0.000000 | **-0.0006** | `-13.5%` | `STOP_LOSS_HIT` | $0.0700 |
| 5 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:10:40 UTC | 40.7s | `1.661` | `1.658` | $0.33 | $0.00 | $0.000000 | **-0.0006** | `-13.5%` | `STOP_LOSS_HIT` | $0.0694 |
| 6 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:04 UTC | 4.5s | `1.645` | `1.648` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.7%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 7 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:24:25 UTC | 1m 25s | `1.658` | `1.655` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.6%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 8 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:35:33 UTC | 33.8s | `1.658` | `1.661` | $0.33 | $0.00 | $0.000000 | **-0.0006** | `-13.6%` | `STOP_LOSS_HIT` | $0.0700 |
| 9 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:12 UTC | 2m 12s | `1.676` | `1.673` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.4%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 10 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:55 UTC | 55.0s | `1.676` | `1.679` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.4%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 11 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:01:16 UTC | 2m 16s | `1.678` | `1.681` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.4%` | `STOP_LOSS_HIT` | $0.0706 |
| 12 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:04:36 UTC | 36.0s | `1.685` | `1.682` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.4%` | `STOP_LOSS_HIT` | $0.0700 |
| 13 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:10:04 UTC | 1m 04s | `1.684` | `1.687` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.4%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 14 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:18:17 UTC | 17.5s | `1.702` | `1.705` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.2%` | `STOP_LOSS_HIT` | $0.0700 |
| 15 | `LONG` | 2026-07-01 02:22:59 UTC | 2026-07-01 02:23:00 UTC | 0.9s | `1.709` | `1.706` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.2%` | `STOP_LOSS_HIT` | $0.0694 |
| 16 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:14 UTC | 1m 14s | `1.705` | `1.708` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 17 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:29 UTC | 29.4s | `1.704` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 18 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:05 UTC | 3m 05s | `1.697` | `1.700` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.3%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 19 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:33 UTC | 33.3s | `1.704` | `1.707` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.2%` | `STOP_LOSS_HIT` | $0.0706 |
| 20 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:07 UTC | 7.4s | `1.707` | `1.710` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.2%` | `STOP_LOSS_HIT` | $0.0700 |
| 21 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:08 UTC | 8.8s | `1.729` | `1.726` | $0.35 | $0.00 | $0.000000 | **+0.0006** | `+13.0%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 22 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:00 UTC | 0.7s | `1.711` | `1.708` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.2%` | `STOP_LOSS_HIT` | $0.0700 |
| 23 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:20:11 UTC | 11.2s | `1.704` | `1.701` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.2%` | `STOP_LOSS_HIT` | $0.0694 |
| 24 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:29:10 UTC | 1m 10s | `1.699` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 25 | `SHORT` | 2026-07-01 03:32:59 UTC | 2026-07-01 03:36:33 UTC | 3m 33s | `1.699` | `1.702` | $0.34 | $0.00 | $0.000000 | **-0.0006** | `-13.2%` | `STOP_LOSS_HIT` | $0.0694 |
| ... | ... | *(3166 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 3192 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:38:55 UTC | 9m 55s | `1.616` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.1324 |
| 3193 | `LONG` | 2026-07-23 19:40:59 UTC | 2026-07-23 19:49:12 UTC | 8m 12s | `1.613` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-13.9%` | `STOP_LOSS_HIT` | $0.1318 |
| 3194 | `LONG` | 2026-07-23 19:52:59 UTC | 2026-07-23 19:56:47 UTC | 3m 47s | `1.609` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1324 |
| 3195 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.1330 |
| 3196 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 20:33:41 UTC | 5m 41s | `1.623` | `1.620` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-13.9%` | `STOP_LOSS_HIT` | $0.1324 |
| 3197 | `LONG` | 2026-07-23 20:45:59 UTC | 2026-07-23 20:50:54 UTC | 4m 54s | `1.618` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.1330 |
| 3198 | `SHORT` | 2026-07-23 20:52:59 UTC | 2026-07-23 20:57:43 UTC | 4m 43s | `1.621` | `1.624` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-13.9%` | `STOP_LOSS_HIT` | $0.1324 |
| 3199 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:08:20 UTC | 2m 20s | `1.622` | `1.619` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.1330 |
| 3200 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:18:08 UTC | 8.4s | `1.617` | `1.614` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-13.9%` | `STOP_LOSS_HIT` | $0.1324 |
| 3201 | `LONG` | 2026-07-23 21:22:59 UTC | 2026-07-23 21:29:06 UTC | 6m 06s | `1.614` | `1.611` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-13.9%` | `STOP_LOSS_HIT` | $0.1318 |
| 3202 | `SHORT` | 2026-07-23 21:30:59 UTC | 2026-07-23 21:32:14 UTC | 1m 14s | `1.610` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1324 |
| 3203 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:44:51 UTC | 6m 51s | `1.603` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1330 |
| 3204 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 21:46:26 UTC | 26.3s | `1.605` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-14.0%` | `STOP_LOSS_HIT` | $0.1324 |
| 3205 | `SHORT` | 2026-07-23 21:48:59 UTC | 2026-07-23 21:55:30 UTC | 6m 30s | `1.605` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-14.0%` | `STOP_LOSS_HIT` | $0.1318 |
| 3206 | `SHORT` | 2026-07-23 22:00:59 UTC | 2026-07-23 22:05:09 UTC | 4m 09s | `1.609` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-14.0%` | `STOP_LOSS_HIT` | $0.1312 |
| 3207 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:55 UTC | 5m 55s | `1.611` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1318 |
| 3208 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:49 UTC | 49.6s | `1.607` | `1.610` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1324 |
| 3209 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:40 UTC | 40.9s | `1.610` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1330 |
| 3210 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.1336 |
| 3211 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:37:16 UTC | 2m 16s | `1.611` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-14.0%` | `STOP_LOSS_HIT` | $0.1330 |
| 3212 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:41:44 UTC | 44.4s | `1.604` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1336 |
| 3213 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:40 UTC | 11m 40s | `1.607` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1342 |
| 3214 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:22:40 UTC | 13m 40s | `1.605` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1348 |
| 3215 | `SHORT` | 2026-07-23 23:24:59 UTC | 2026-07-23 23:47:35 UTC | 22m 35s | `1.607` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1354 |
| 3216 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:03:59 UTC | 8m 59s | `1.599` | `1.596` | $0.32 | $0.00 | $0.000000 | **-0.0006** | `-14.1%` | `STOP_LOSS_HIT` | $0.1348 |

> 💡 *Full granular dataset with all 3216 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
