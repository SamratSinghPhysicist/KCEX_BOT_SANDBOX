# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:10:42 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.2142 USDT` | `₹20.23` | `+206.00%` |
| **Net Realized PnL** | **`+0.1442 USDT`** | **`₹+13.62`** | **`+206.00% Net ROI`** |
| **Gross Profit** | `+1.0122 USDT` | `₹95.60` | Total positive trade returns |
| **Gross Loss** | `-0.8680 USDT` | `₹81.98` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.17`** | — | Profitable |
| **Win / Loss Payoff** | `0.60` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0174 USDT` | `₹1.64` | **`-22.10%` Peak-to-Trough** |
| **Win Rate** | **`66.03%`** | — | `1687 Wins / 868 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `5.26` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `3.99` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `9.32` | — | Net ROI divided by Max Drawdown |

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
| **Total Trades Executed** | `2555` | Total completed trade lifecycle events |
| **Winning Trades** | `1687` | `66.03%` of total trades |
| **Losing Trades** | `868` | `33.97%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0001 USDT` (`₹+0.01`) | Expected return per signal |
| **Average Winning Trade** | `+0.0006 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0010 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0006 USDT (+13.5% ROE)` | Trade #3 (SHORT) |
| **Largest Losing Trade** | `-0.0010 USDT (-22.5% ROE)` | Trade #2 (SHORT) |
| **Max Consecutive Wins** | `25` trades | Peak winning streak |
| **Max Consecutive Losses** | `7` trades | Peak losing streak |
| **Average Trade Duration** | `7m 14s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #261 |
| **Longest Trade In-Position** | `2h 07m 06s` | Trade #1287 |
| **Cumulative Time In Position** | `308h 42m 21s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1253` (49.0%) | `1302` (51.0%) | `2555` |
| **Wins / Losses** | `826 W / 427 L` | `861 W / 441 L` | `1687 W / 868 L` |
| **Win Rate** | **`65.92%`** | **`66.13%`** | **`66.03%`** |
| **Gross Profit** | `+0.4956 USDT` | `+0.5166 USDT` | `+1.0122 USDT` |
| **Gross Loss** | `-0.4270 USDT` | `-0.4410 USDT` | `-0.8680 USDT` |
| **Net Realized PnL** | **`+0.0686 USDT`** | **`+0.0756 USDT`** | **`+0.1442 USDT`** |
| **Net PnL (INR)** | `₹+6.48` | `₹+7.14` | `₹+13.62` |
| **Profit Factor** | `1.16` | `1.17` | `1.17` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1687` | `66.0%` | `+1.0122 USDT` | `₹+95.60` | `100.0%` | `6m 18s` |
| `STOP_LOSS_HIT` | `868` | `34.0%` | `-0.8680 USDT` | `₹-81.98` | `0.0%` | `9m 03s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:30:42 UTC | 1m 42s | `1.661` | `1.664` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.5%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:52:44 UTC | 15m 44s | `1.664` | `1.669` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.5%` | `STOP_LOSS_HIT` | $0.0696 |
| 3 | `SHORT` | 2026-07-01 00:55:59 UTC | 2026-07-01 00:56:42 UTC | 42.7s | `1.669` | `1.666` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.5%` | `MIN_PROFIT_TP_HIT` | $0.0702 |
| 4 | `LONG` | 2026-07-01 01:01:59 UTC | 2026-07-01 01:05:16 UTC | 3m 16s | `1.667` | `1.662` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.5%` | `STOP_LOSS_HIT` | $0.0692 |
| 5 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:11:30 UTC | 1m 30s | `1.661` | `1.656` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.6%` | `STOP_LOSS_HIT` | $0.0682 |
| 6 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:04 UTC | 4.5s | `1.645` | `1.648` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.7%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 7 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:24:25 UTC | 1m 25s | `1.658` | `1.655` | $0.33 | $0.00 | $0.000000 | **+0.0006** | `+13.6%` | `MIN_PROFIT_TP_HIT` | $0.0694 |
| 8 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:36:14 UTC | 1m 14s | `1.658` | `1.663` | $0.33 | $0.00 | $0.000000 | **-0.0010** | `-22.6%` | `STOP_LOSS_HIT` | $0.0684 |
| 9 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:12 UTC | 2m 12s | `1.676` | `1.673` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.4%` | `MIN_PROFIT_TP_HIT` | $0.0690 |
| 10 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:55 UTC | 55.0s | `1.676` | `1.679` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.4%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 11 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:02:36 UTC | 3m 36s | `1.678` | `1.683` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.3%` | `STOP_LOSS_HIT` | $0.0686 |
| 12 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:05:51 UTC | 1m 51s | `1.685` | `1.680` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.3%` | `STOP_LOSS_HIT` | $0.0676 |
| 13 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:10:04 UTC | 1m 04s | `1.684` | `1.687` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.4%` | `MIN_PROFIT_TP_HIT` | $0.0682 |
| 14 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:22:04 UTC | 4m 04s | `1.702` | `1.707` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0672 |
| 15 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:14 UTC | 1m 14s | `1.705` | `1.708` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0678 |
| 16 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:29 UTC | 29.4s | `1.704` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 17 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:05 UTC | 3m 05s | `1.697` | `1.700` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.3%` | `MIN_PROFIT_TP_HIT` | $0.0690 |
| 18 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:34 UTC | 34.2s | `1.704` | `1.709` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0680 |
| 19 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:07 UTC | 7.4s | `1.707` | `1.712` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0670 |
| 20 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:08 UTC | 8.8s | `1.729` | `1.726` | $0.35 | $0.00 | $0.000000 | **+0.0006** | `+13.0%` | `MIN_PROFIT_TP_HIT` | $0.0676 |
| 21 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:12 UTC | 12.1s | `1.711` | `1.706` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-21.9%` | `STOP_LOSS_HIT` | $0.0666 |
| 22 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:23:46 UTC | 3m 46s | `1.704` | `1.699` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0656 |
| 23 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:29:10 UTC | 1m 10s | `1.699` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0006** | `+13.2%` | `MIN_PROFIT_TP_HIT` | $0.0662 |
| 24 | `SHORT` | 2026-07-01 03:32:59 UTC | 2026-07-01 03:36:50 UTC | 3m 50s | `1.699` | `1.704` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.1%` | `STOP_LOSS_HIT` | $0.0652 |
| 25 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:47:01 UTC | 5m 01s | `1.706` | `1.711` | $0.34 | $0.00 | $0.000000 | **-0.0010** | `-22.0%` | `STOP_LOSS_HIT` | $0.0642 |
| ... | ... | *(2505 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2531 | `LONG` | 2026-07-23 18:40:59 UTC | 2026-07-23 18:52:55 UTC | 11m 55s | `1.608` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2158 |
| 2532 | `SHORT` | 2026-07-23 18:56:59 UTC | 2026-07-23 19:25:52 UTC | 28m 52s | `1.610` | `1.615` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.2148 |
| 2533 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:38:55 UTC | 9m 55s | `1.616` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.2154 |
| 2534 | `LONG` | 2026-07-23 19:40:59 UTC | 2026-07-23 19:50:07 UTC | 9m 07s | `1.613` | `1.608` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.2144 |
| 2535 | `LONG` | 2026-07-23 19:52:59 UTC | 2026-07-23 19:56:47 UTC | 3m 47s | `1.609` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2150 |
| 2536 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.2156 |
| 2537 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 20:40:43 UTC | 12m 43s | `1.623` | `1.618` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.2146 |
| 2538 | `LONG` | 2026-07-23 20:45:59 UTC | 2026-07-23 20:50:54 UTC | 4m 54s | `1.618` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.2152 |
| 2539 | `SHORT` | 2026-07-23 20:52:59 UTC | 2026-07-23 21:04:40 UTC | 11m 40s | `1.621` | `1.626` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.1%` | `STOP_LOSS_HIT` | $0.2142 |
| 2540 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:08:20 UTC | 2m 20s | `1.622` | `1.619` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.2148 |
| 2541 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:18:27 UTC | 27.3s | `1.617` | `1.612` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.2138 |
| 2542 | `LONG` | 2026-07-23 21:22:59 UTC | 2026-07-23 21:31:59 UTC | 8m 59s | `1.614` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.2%` | `STOP_LOSS_HIT` | $0.2128 |
| 2543 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:44:51 UTC | 6m 51s | `1.603` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2134 |
| 2544 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 21:56:25 UTC | 10m 25s | `1.605` | `1.610` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.4%` | `STOP_LOSS_HIT` | $0.2124 |
| 2545 | `SHORT` | 2026-07-23 22:00:59 UTC | 2026-07-23 22:06:32 UTC | 5m 32s | `1.609` | `1.614` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.2114 |
| 2546 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:55 UTC | 5m 55s | `1.611` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2120 |
| 2547 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:49 UTC | 49.6s | `1.607` | `1.610` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2126 |
| 2548 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:40 UTC | 40.9s | `1.610` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2132 |
| 2549 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.613` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+13.9%` | `MIN_PROFIT_TP_HIT` | $0.2138 |
| 2550 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:37:30 UTC | 2m 30s | `1.611` | `1.606` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.3%` | `STOP_LOSS_HIT` | $0.2128 |
| 2551 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:41:44 UTC | 44.4s | `1.604` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2134 |
| 2552 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:40 UTC | 11m 40s | `1.607` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2140 |
| 2553 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:22:40 UTC | 13m 40s | `1.605` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2146 |
| 2554 | `SHORT` | 2026-07-23 23:24:59 UTC | 2026-07-23 23:47:35 UTC | 22m 35s | `1.607` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0006** | `+14.0%` | `MIN_PROFIT_TP_HIT` | $0.2152 |
| 2555 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:05:13 UTC | 10m 13s | `1.599` | `1.594` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.5%` | `STOP_LOSS_HIT` | $0.2142 |

> 💡 *Full granular dataset with all 2555 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
