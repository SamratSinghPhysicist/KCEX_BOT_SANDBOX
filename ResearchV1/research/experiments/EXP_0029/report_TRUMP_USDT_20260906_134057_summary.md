# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:10:57 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.1924 USDT` | `₹18.17` | `+174.86%` |
| **Net Realized PnL** | **`+0.1224 USDT`** | **`₹+11.56`** | **`+174.86% Net ROI`** |
| **Gross Profit** | `+0.9888 USDT` | `₹93.39` | Total positive trade returns |
| **Gross Loss** | `-0.8664 USDT` | `₹81.83` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.14`** | — | Profitable |
| **Win / Loss Payoff** | `0.50` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0240 USDT` | `₹2.27` | **`-33.99%` Peak-to-Trough** |
| **Win Rate** | **`69.54%`** | — | `1648 Wins / 722 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `4.48` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `3.09` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `5.14` | — | Net ROI divided by Max Drawdown |

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
| **Stop Loss Rule** | `-6 ticks away from entry (0.006 USDT)` | Stop loss evaluation logic |

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
| **Total Trades Executed** | `2370` | Total completed trade lifecycle events |
| **Winning Trades** | `1648` | `69.54%` of total trades |
| **Losing Trades** | `722` | `30.46%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0001 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0006 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0012 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0006 USDT (+13.5% ROE)` | Trade #3 (SHORT) |
| **Largest Losing Trade** | `-0.0012 USDT (-27.0% ROE)` | Trade #2 (SHORT) |
| **Max Consecutive Wins** | `25` trades | Peak winning streak |
| **Max Consecutive Losses** | `6` trades | Peak losing streak |
| **Average Trade Duration** | `8m 20s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #242 |
| **Longest Trade In-Position** | `2h 07m 06s` | Trade #1193 |
| **Cumulative Time In Position** | `329h 13m 59s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1171` (49.4%) | `1199` (50.6%) | `2370` |
| **Wins / Losses** | `810 W / 361 L` | `838 W / 361 L` | `1648 W / 722 L` |
| **Win Rate** | **`69.17%`** | **`69.89%`** | **`69.54%`** |
| **Gross Profit** | `+0.4860 USDT` | `+0.5028 USDT` | `+0.9888 USDT` |
| **Gross Loss** | `-0.4332 USDT` | `-0.4332 USDT` | `-0.8664 USDT` |
| **Net Realized PnL** | **`+0.0528 USDT`** | **`+0.0696 USDT`** | **`+0.1224 USDT`** |
| **Net PnL (INR)** | `₹+4.99` | `₹+6.57` | `₹+11.56` |
| **Profit Factor** | `1.12` | `1.16` | `1.14` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1648` | `69.5%` | `+0.9888 USDT` | `₹+93.39` | `100.0%` | `6m 58s` |
| `STOP_LOSS_HIT` | `722` | `30.5%` | `-0.8664 USDT` | `₹-81.83` | `0.0%` | `11m 27s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:30:42 UTC | 1m 42s | `1.661` | `1.664` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.5%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:52:46 UTC | 15m 46s | `1.664` | `1.670` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.0%` | `STOP_LOSS_HIT` | $0.0694 |
| 3 | `SHORT` | 2026-07-01 00:55:59 UTC | 2026-07-01 00:56:42 UTC | 42.7s | `1.669` | `1.666` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.5%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 4 | `LONG` | 2026-07-01 01:01:59 UTC | 2026-07-01 01:07:03 UTC | 5m 03s | `1.667` | `1.661` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.0%` | `STOP_LOSS_HIT` | $0.0688 |
| 5 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:12:29 UTC | 2m 29s | `1.661` | `1.655` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.1%` | `STOP_LOSS_HIT` | $0.0676 |
| 6 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:04 UTC | 4.5s | `1.645` | `1.648` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.7%` | `MIN_PROFIT_TP_HIT` | $0.0682 |
| 7 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:24:25 UTC | 1m 25s | `1.658` | `1.655` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.6%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 8 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:37:07 UTC | 2m 07s | `1.658` | `1.664` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.1%` | `STOP_LOSS_HIT` | $0.0676 |
| 9 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:12 UTC | 2m 12s | `1.676` | `1.673` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.4%` | `MIN_PROFIT_TP_HIT` | $0.0682 |
| 10 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:55 UTC | 55.0s | `1.676` | `1.679` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.4%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 11 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:02:52 UTC | 3m 52s | `1.678` | `1.684` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.8%` | `STOP_LOSS_HIT` | $0.0676 |
| 12 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:06:09 UTC | 2m 09s | `1.685` | `1.679` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.7%` | `STOP_LOSS_HIT` | $0.0664 |
| 13 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:10:04 UTC | 1m 04s | `1.684` | `1.687` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.4%` | `MIN_PROFIT_TP_HIT` | $0.0670 |
| 14 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:22:05 UTC | 4m 05s | `1.702` | `1.708` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0658 |
| 15 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:14 UTC | 1m 14s | `1.705` | `1.708` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0664 |
| 16 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:29 UTC | 29.4s | `1.704` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0670 |
| 17 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:05 UTC | 3m 05s | `1.697` | `1.700` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.3%` | `MIN_PROFIT_TP_HIT` | $0.0676 |
| 18 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:38 UTC | 38.4s | `1.704` | `1.710` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0664 |
| 19 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:24 UTC | 24.3s | `1.707` | `1.713` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0652 |
| 20 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:08 UTC | 8.8s | `1.729` | `1.726` | $0.35 | $0.00 | $0.000000 | **+0.0006** | `+13.0%` | `MIN_PROFIT_TP_HIT` | $0.0658 |
| 21 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:27 UTC | 28.0s | `1.711` | `1.705` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.3%` | `STOP_LOSS_HIT` | $0.0646 |
| 22 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:23:46 UTC | 3m 46s | `1.704` | `1.698` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0634 |
| 23 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:29:10 UTC | 1m 10s | `1.699` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0640 |
| 24 | `SHORT` | 2026-07-01 03:32:59 UTC | 2026-07-01 03:37:04 UTC | 4m 04s | `1.699` | `1.705` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.5%` | `STOP_LOSS_HIT` | $0.0628 |
| 25 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:47:31 UTC | 5m 31s | `1.706` | `1.712` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0616 |
| ... | ... | *(2320 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2346 | `LONG` | 2026-07-23 18:02:59 UTC | 2026-07-23 18:05:38 UTC | 2m 38s | `1.599` | `1.593` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-28.1%` | `STOP_LOSS_HIT` | $0.1888 |
| 2347 | `SHORT` | 2026-07-23 18:12:59 UTC | 2026-07-23 18:17:24 UTC | 4m 24s | `1.594` | `1.591` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.1%` | `MIN_PROFIT_TP_HIT` | $0.1894 |
| 2348 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:37:12 UTC | 8m 12s | `1.610` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1900 |
| 2349 | `LONG` | 2026-07-23 18:40:59 UTC | 2026-07-23 18:52:55 UTC | 11m 55s | `1.608` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1906 |
| 2350 | `SHORT` | 2026-07-23 18:56:59 UTC | 2026-07-23 19:25:52 UTC | 28m 52s | `1.610` | `1.616` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-28.0%` | `STOP_LOSS_HIT` | $0.1894 |
| 2351 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:38:55 UTC | 9m 55s | `1.616` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.1900 |
| 2352 | `LONG` | 2026-07-23 19:40:59 UTC | 2026-07-23 19:51:13 UTC | 10m 13s | `1.613` | `1.607` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-27.9%` | `STOP_LOSS_HIT` | $0.1888 |
| 2353 | `LONG` | 2026-07-23 19:52:59 UTC | 2026-07-23 19:56:47 UTC | 3m 47s | `1.609` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1894 |
| 2354 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.1900 |
| 2355 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 21:04:40 UTC | 36m 40s | `1.623` | `1.626` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.1906 |
| 2356 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:08:20 UTC | 2m 20s | `1.622` | `1.619` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.1912 |
| 2357 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:29:06 UTC | 11m 06s | `1.617` | `1.611` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-27.8%` | `STOP_LOSS_HIT` | $0.1900 |
| 2358 | `SHORT` | 2026-07-23 21:30:59 UTC | 2026-07-23 21:32:14 UTC | 1m 14s | `1.610` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1906 |
| 2359 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:44:51 UTC | 6m 51s | `1.603` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1912 |
| 2360 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 22:05:02 UTC | 19m 02s | `1.605` | `1.611` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-28.0%` | `STOP_LOSS_HIT` | $0.1900 |
| 2361 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:55 UTC | 5m 55s | `1.611` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1906 |
| 2362 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:49 UTC | 49.6s | `1.607` | `1.610` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1912 |
| 2363 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:40 UTC | 40.9s | `1.610` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1918 |
| 2364 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.1924 |
| 2365 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:37:43 UTC | 2m 43s | `1.611` | `1.605` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-27.9%` | `STOP_LOSS_HIT` | $0.1912 |
| 2366 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:41:44 UTC | 44.4s | `1.604` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1918 |
| 2367 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:40 UTC | 11m 40s | `1.607` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1924 |
| 2368 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:22:40 UTC | 13m 40s | `1.605` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1930 |
| 2369 | `SHORT` | 2026-07-23 23:24:59 UTC | 2026-07-23 23:47:35 UTC | 22m 35s | `1.607` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.1936 |
| 2370 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:05:54 UTC | 10m 54s | `1.599` | `1.593` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-28.1%` | `STOP_LOSS_HIT` | $0.1924 |

> 💡 *Full granular dataset with all 2370 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
