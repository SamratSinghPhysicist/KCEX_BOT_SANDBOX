# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:03:48 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.2412 USDT` | `₹22.78` | `+244.57%` |
| **Net Realized PnL** | **`+0.1712 USDT`** | **`₹+16.17`** | **`+244.57% Net ROI`** |
| **Gross Profit** | `+0.7912 USDT` | `₹74.73` | Total positive trade returns |
| **Gross Loss** | `-0.6200 USDT` | `₹58.56` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.28`** | — | Profitable |
| **Win / Loss Payoff** | `0.20` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0196 USDT` | `₹1.85` | **`-15.89%` Peak-to-Trough** |
| **Win Rate** | **`86.45%`** | — | `1978 Wins / 310 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `7.55` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `3.12` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `15.39` | — | Net ROI divided by Max Drawdown |

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
| **Stop Loss Rule** | `-10 ticks away from entry (0.010 USDT)` | Stop loss evaluation logic |

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
| **Total Trades Executed** | `2288` | Total completed trade lifecycle events |
| **Winning Trades** | `1978` | `86.45%` of total trades |
| **Losing Trades** | `310` | `13.55%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0001 USDT` (`₹+0.01`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0020 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0020 USDT (-45.2% ROE)` | Trade #3 (LONG) |
| **Max Consecutive Wins** | `49` trades | Peak winning streak |
| **Max Consecutive Losses** | `3` trades | Peak losing streak |
| **Average Trade Duration** | `8m 26s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #1451 |
| **Longest Trade In-Position** | `3h 46m 53s` | Trade #1712 |
| **Cumulative Time In Position** | `322h 05m 46s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1137` (49.7%) | `1151` (50.3%) | `2288` |
| **Wins / Losses** | `973 W / 164 L` | `1005 W / 146 L` | `1978 W / 310 L` |
| **Win Rate** | **`85.58%`** | **`87.32%`** | **`86.45%`** |
| **Gross Profit** | `+0.3892 USDT` | `+0.4020 USDT` | `+0.7912 USDT` |
| **Gross Loss** | `-0.3280 USDT` | `-0.2920 USDT` | `-0.6200 USDT` |
| **Net Realized PnL** | **`+0.0612 USDT`** | **`+0.1100 USDT`** | **`+0.1712 USDT`** |
| **Net PnL (INR)** | `₹+5.78` | `₹+10.39` | `₹+16.17` |
| **Profit Factor** | `1.19` | `1.38` | `1.28` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1978` | `86.5%` | `+0.7912 USDT` | `₹+74.73` | `100.0%` | `6m 08s` |
| `STOP_LOSS_HIT` | `310` | `13.5%` | `-0.6200 USDT` | `₹-58.56` | `0.0%` | `23m 06s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:29:47 UTC | 47.6s | `1.661` | `1.663` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 01:05:16 UTC | 28m 16s | `1.664` | `1.662` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 3 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:12:45 UTC | 2m 45s | `1.661` | `1.651` | $0.33 | $0.00 | $0.000000 | **-0.0020** | `-45.2%` | `STOP_LOSS_HIT` | $0.0688 |
| 4 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:03 UTC | 3.2s | `1.645` | `1.647` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 5 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:23:12 UTC | 12.6s | `1.658` | `1.656` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 6 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:38:46 UTC | 3m 46s | `1.658` | `1.668` | $0.33 | $0.00 | $0.000000 | **-0.0020** | `-45.2%` | `STOP_LOSS_HIT` | $0.0676 |
| 7 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:09 UTC | 2m 09s | `1.676` | `1.674` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0680 |
| 8 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:10 UTC | 10.2s | `1.676` | `1.678` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 9 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:10:07 UTC | 11m 07s | `1.678` | `1.688` | $0.34 | $0.00 | $0.000000 | **-0.0020** | `-44.7%` | `STOP_LOSS_HIT` | $0.0664 |
| 10 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:37:07 UTC | 19m 07s | `1.702` | `1.700` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 11 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:01 UTC | 3m 01s | `1.697` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0672 |
| 12 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:05:28 UTC | 4m 28s | `1.704` | `1.714` | $0.34 | $0.00 | $0.000000 | **-0.0020** | `-44.0%` | `STOP_LOSS_HIT` | $0.0652 |
| 13 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:04 UTC | 4.8s | `1.729` | `1.727` | $0.35 | $0.00 | $0.000000 | **+0.0004** | `+8.7%` | `MIN_PROFIT_TP_HIT` | $0.0656 |
| 14 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:17:39 UTC | 1m 39s | `1.711` | `1.701` | $0.34 | $0.00 | $0.000000 | **-0.0020** | `-43.8%` | `STOP_LOSS_HIT` | $0.0636 |
| 15 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:37:08 UTC | 17m 08s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0640 |
| 16 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:48:40 UTC | 6m 40s | `1.706` | `1.704` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0644 |
| 17 | `LONG` | 2026-07-01 03:51:59 UTC | 2026-07-01 03:52:16 UTC | 16.2s | `1.711` | `1.713` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0648 |
| 18 | `SHORT` | 2026-07-01 03:56:59 UTC | 2026-07-01 03:57:03 UTC | 3.5s | `1.712` | `1.710` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 19 | `LONG` | 2026-07-01 04:02:59 UTC | 2026-07-01 04:04:04 UTC | 1m 04s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0656 |
| 20 | `LONG` | 2026-07-01 04:11:59 UTC | 2026-07-01 04:16:02 UTC | 4m 02s | `1.700` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0660 |
| 21 | `SHORT` | 2026-07-01 04:21:59 UTC | 2026-07-01 04:23:55 UTC | 1m 55s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0664 |
| 22 | `LONG` | 2026-07-01 04:27:59 UTC | 2026-07-01 04:31:23 UTC | 3m 23s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 23 | `LONG` | 2026-07-01 04:38:59 UTC | 2026-07-01 04:41:01 UTC | 2m 01s | `1.700` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0672 |
| 24 | `SHORT` | 2026-07-01 04:59:59 UTC | 2026-07-01 05:00:10 UTC | 10.4s | `1.704` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0676 |
| 25 | `LONG` | 2026-07-01 05:06:59 UTC | 2026-07-01 05:12:42 UTC | 5m 42s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0680 |
| ... | ... | *(2238 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2264 | `SHORT` | 2026-07-23 16:17:59 UTC | 2026-07-23 16:18:39 UTC | 40.0s | `1.643` | `1.641` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.2532 |
| 2265 | `LONG` | 2026-07-23 16:22:59 UTC | 2026-07-23 16:24:16 UTC | 1m 16s | `1.642` | `1.644` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.2536 |
| 2266 | `LONG` | 2026-07-23 16:34:59 UTC | 2026-07-23 16:36:24 UTC | 1m 24s | `1.639` | `1.641` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2540 |
| 2267 | `LONG` | 2026-07-23 16:37:59 UTC | 2026-07-23 16:45:58 UTC | 7m 58s | `1.641` | `1.631` | $0.33 | $0.00 | $0.000000 | **-0.0020** | `-45.7%` | `STOP_LOSS_HIT` | $0.2520 |
| 2268 | `LONG` | 2026-07-23 16:58:59 UTC | 2026-07-23 17:02:07 UTC | 3m 07s | `1.631` | `1.621` | $0.33 | $0.00 | $0.000000 | **-0.0020** | `-46.0%` | `STOP_LOSS_HIT` | $0.2500 |
| 2269 | `LONG` | 2026-07-23 17:04:59 UTC | 2026-07-23 17:40:48 UTC | 35m 48s | `1.621` | `1.611` | $0.32 | $0.00 | $0.000000 | **-0.0020** | `-46.3%` | `STOP_LOSS_HIT` | $0.2480 |
| 2270 | `SHORT` | 2026-07-23 17:47:59 UTC | 2026-07-23 17:53:13 UTC | 5m 13s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2484 |
| 2271 | `LONG` | 2026-07-23 18:02:59 UTC | 2026-07-23 18:17:39 UTC | 14m 39s | `1.599` | `1.589` | $0.32 | $0.00 | $0.000000 | **-0.0020** | `-46.9%` | `STOP_LOSS_HIT` | $0.2464 |
| 2272 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:30:28 UTC | 1m 28s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2468 |
| 2273 | `LONG` | 2026-07-23 18:35:59 UTC | 2026-07-23 19:02:40 UTC | 26m 40s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2472 |
| 2274 | `SHORT` | 2026-07-23 19:06:59 UTC | 2026-07-23 19:25:52 UTC | 18m 52s | `1.609` | `1.619` | $0.32 | $0.00 | $0.000000 | **-0.0020** | `-46.6%` | `STOP_LOSS_HIT` | $0.2452 |
| 2275 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:29:04 UTC | 4.2s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2456 |
| 2276 | `LONG` | 2026-07-23 19:40:59 UTC | 2026-07-23 19:58:16 UTC | 17m 16s | `1.613` | `1.615` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2460 |
| 2277 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2464 |
| 2278 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 21:01:39 UTC | 33m 39s | `1.623` | `1.625` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2468 |
| 2279 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:07:45 UTC | 1m 45s | `1.622` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2472 |
| 2280 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:32:14 UTC | 14m 14s | `1.617` | `1.607` | $0.32 | $0.00 | $0.000000 | **-0.0020** | `-46.4%` | `STOP_LOSS_HIT` | $0.2452 |
| 2281 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:38:30 UTC | 30.0s | `1.603` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2456 |
| 2282 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 22:07:08 UTC | 21m 08s | `1.605` | `1.615` | $0.32 | $0.00 | $0.000000 | **-0.0020** | `-46.7%` | `STOP_LOSS_HIT` | $0.2436 |
| 2283 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:17 UTC | 5m 17s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2440 |
| 2284 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:24 UTC | 24.5s | `1.607` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2444 |
| 2285 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:20 UTC | 20.1s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2448 |
| 2286 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2452 |
| 2287 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 23:51:57 UTC | 1h 16m 57s | `1.611` | `1.601` | $0.32 | $0.00 | $0.000000 | **-0.0020** | `-46.6%` | `STOP_LOSS_HIT` | $0.2432 |
| 2288 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:07:16 UTC | 12m 16s | `1.599` | `1.589` | $0.32 | $0.00 | $0.000000 | **-0.0020** | `-46.9%` | `STOP_LOSS_HIT` | $0.2412 |

> 💡 *Full granular dataset with all 2288 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
