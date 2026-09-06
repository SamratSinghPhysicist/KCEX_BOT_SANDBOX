# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:03:31 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.2588 USDT` | `₹24.44` | `+269.71%` |
| **Net Realized PnL** | **`+0.1888 USDT`** | **`₹+17.83`** | **`+269.71% Net ROI`** |
| **Gross Profit** | `+0.8576 USDT` | `₹81.00` | Total positive trade returns |
| **Gross Loss** | `-0.6688 USDT` | `₹63.17` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.28`** | — | Profitable |
| **Win / Loss Payoff** | `0.25` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0220 USDT` | `₹2.08` | **`-14.03%` Peak-to-Trough** |
| **Win Rate** | **`83.68%`** | — | `2144 Wins / 418 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `8.38` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `3.91` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `19.23` | — | Net ROI divided by Max Drawdown |

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
| **Stop Loss Rule** | `-8 ticks away from entry (0.008 USDT)` | Stop loss evaluation logic |

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
| **Total Trades Executed** | `2562` | Total completed trade lifecycle events |
| **Winning Trades** | `2144` | `83.68%` of total trades |
| **Losing Trades** | `418` | `16.32%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0001 USDT` (`₹+0.01`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0016 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.0% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0016 USDT (-36.1% ROE)` | Trade #3 (LONG) |
| **Max Consecutive Wins** | `51` trades | Peak winning streak |
| **Max Consecutive Losses** | `5` trades | Peak losing streak |
| **Average Trade Duration** | `6m 54s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #1578 |
| **Longest Trade In-Position** | `2h 22m 33s` | Trade #1448 |
| **Cumulative Time In Position** | `294h 53m 06s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1276` (49.8%) | `1286` (50.2%) | `2562` |
| **Wins / Losses** | `1052 W / 224 L` | `1092 W / 194 L` | `2144 W / 418 L` |
| **Win Rate** | **`82.45%`** | **`84.91%`** | **`83.68%`** |
| **Gross Profit** | `+0.4208 USDT` | `+0.4368 USDT` | `+0.8576 USDT` |
| **Gross Loss** | `-0.3584 USDT` | `-0.3104 USDT` | `-0.6688 USDT` |
| **Net Realized PnL** | **`+0.0624 USDT`** | **`+0.1264 USDT`** | **`+0.1888 USDT`** |
| **Net PnL (INR)** | `₹+5.89` | `₹+11.94` | `₹+17.83` |
| **Profit Factor** | `1.17` | `1.41` | `1.28` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `2144` | `83.7%` | `+0.8576 USDT` | `₹+81.00` | `100.0%` | `5m 07s` |
| `STOP_LOSS_HIT` | `418` | `16.3%` | `-0.6688 USDT` | `₹-63.17` | `0.0%` | `16m 00s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:29:47 UTC | 47.6s | `1.661` | `1.663` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 01:05:16 UTC | 28m 16s | `1.664` | `1.662` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 3 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:12:44 UTC | 2m 44s | `1.661` | `1.653` | $0.33 | $0.00 | $0.000000 | **-0.0016** | `-36.1%` | `STOP_LOSS_HIT` | $0.0692 |
| 4 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:03 UTC | 3.2s | `1.645` | `1.647` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.1%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 5 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:23:12 UTC | 12.6s | `1.658` | `1.656` | $0.33 | $0.00 | $0.000000 | **+0.0004** | `+9.0%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 6 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:38:45 UTC | 3m 45s | `1.658` | `1.666` | $0.33 | $0.00 | $0.000000 | **-0.0016** | `-36.2%` | `STOP_LOSS_HIT` | $0.0684 |
| 7 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:50:09 UTC | 2m 09s | `1.676` | `1.674` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 8 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:10 UTC | 10.2s | `1.676` | `1.678` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 9 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:03:45 UTC | 4m 45s | `1.678` | `1.686` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.8%` | `STOP_LOSS_HIT` | $0.0676 |
| 10 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:09:39 UTC | 39.7s | `1.684` | `1.686` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.9%` | `MIN_PROFIT_TP_HIT` | $0.0680 |
| 11 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:31:24 UTC | 13m 24s | `1.702` | `1.710` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.3%` | `STOP_LOSS_HIT` | $0.0664 |
| 12 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:05 UTC | 5.7s | `1.704` | `1.706` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 13 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:01 UTC | 3m 01s | `1.697` | `1.699` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0672 |
| 14 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:39 UTC | 39.6s | `1.704` | `1.712` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.2%` | `STOP_LOSS_HIT` | $0.0656 |
| 15 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:32 UTC | 32.4s | `1.707` | `1.715` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.1%` | `STOP_LOSS_HIT` | $0.0640 |
| 16 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:04 UTC | 4.8s | `1.729` | `1.727` | $0.35 | $0.00 | $0.000000 | **+0.0004** | `+8.7%` | `MIN_PROFIT_TP_HIT` | $0.0644 |
| 17 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:30 UTC | 30.3s | `1.711` | `1.703` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.1%` | `STOP_LOSS_HIT` | $0.0628 |
| 18 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:24:02 UTC | 4m 02s | `1.704` | `1.696` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.2%` | `STOP_LOSS_HIT` | $0.0612 |
| 19 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:29:01 UTC | 1m 01s | `1.699` | `1.701` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0616 |
| 20 | `SHORT` | 2026-07-01 03:32:59 UTC | 2026-07-01 03:34:17 UTC | 1m 17s | `1.699` | `1.697` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0620 |
| 21 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:48:40 UTC | 6m 40s | `1.706` | `1.704` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0624 |
| 22 | `LONG` | 2026-07-01 03:51:59 UTC | 2026-07-01 03:52:16 UTC | 16.2s | `1.711` | `1.713` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0628 |
| 23 | `SHORT` | 2026-07-01 03:56:59 UTC | 2026-07-01 03:57:03 UTC | 3.5s | `1.712` | `1.710` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0632 |
| 24 | `LONG` | 2026-07-01 04:02:59 UTC | 2026-07-01 04:04:04 UTC | 1m 04s | `1.705` | `1.707` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0636 |
| 25 | `LONG` | 2026-07-01 04:11:59 UTC | 2026-07-01 04:16:02 UTC | 4m 02s | `1.700` | `1.702` | $0.34 | $0.00 | $0.000000 | **+0.0004** | `+8.8%` | `MIN_PROFIT_TP_HIT` | $0.0640 |
| ... | ... | *(2512 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2538 | `SHORT` | 2026-07-23 17:47:59 UTC | 2026-07-23 17:53:13 UTC | 5m 13s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2612 |
| 2539 | `LONG` | 2026-07-23 18:02:59 UTC | 2026-07-23 18:05:47 UTC | 2m 47s | `1.599` | `1.591` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.5%` | `STOP_LOSS_HIT` | $0.2596 |
| 2540 | `SHORT` | 2026-07-23 18:12:59 UTC | 2026-07-23 18:16:12 UTC | 3m 12s | `1.594` | `1.592` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2600 |
| 2541 | `SHORT` | 2026-07-23 18:17:59 UTC | 2026-07-23 18:18:03 UTC | 3.1s | `1.589` | `1.587` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2604 |
| 2542 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:30:28 UTC | 1m 28s | `1.610` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2608 |
| 2543 | `LONG` | 2026-07-23 18:35:59 UTC | 2026-07-23 19:02:40 UTC | 26m 40s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2612 |
| 2544 | `SHORT` | 2026-07-23 19:06:59 UTC | 2026-07-23 19:25:52 UTC | 18m 52s | `1.609` | `1.617` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.3%` | `STOP_LOSS_HIT` | $0.2596 |
| 2545 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:29:04 UTC | 4.2s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2600 |
| 2546 | `LONG` | 2026-07-23 19:40:59 UTC | 2026-07-23 19:58:16 UTC | 17m 16s | `1.613` | `1.615` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2604 |
| 2547 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:24:57 UTC | 13m 57s | `1.623` | `1.621` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2608 |
| 2548 | `LONG` | 2026-07-23 20:27:59 UTC | 2026-07-23 21:01:39 UTC | 33m 39s | `1.623` | `1.625` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2612 |
| 2549 | `SHORT` | 2026-07-23 21:05:59 UTC | 2026-07-23 21:07:45 UTC | 1m 45s | `1.622` | `1.620` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.2%` | `MIN_PROFIT_TP_HIT` | $0.2616 |
| 2550 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:31:59 UTC | 13m 59s | `1.617` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.1%` | `STOP_LOSS_HIT` | $0.2600 |
| 2551 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:38:30 UTC | 30.0s | `1.603` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2604 |
| 2552 | `SHORT` | 2026-07-23 21:45:59 UTC | 2026-07-23 22:06:10 UTC | 20m 10s | `1.605` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.4%` | `STOP_LOSS_HIT` | $0.2588 |
| 2553 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:17 UTC | 5m 17s | `1.611` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2592 |
| 2554 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:19:24 UTC | 24.5s | `1.607` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2596 |
| 2555 | `LONG` | 2026-07-23 22:20:59 UTC | 2026-07-23 22:21:20 UTC | 20.1s | `1.610` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2600 |
| 2556 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:29:23 UTC | 1m 23s | `1.616` | `1.614` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2604 |
| 2557 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:38:25 UTC | 3m 25s | `1.611` | `1.603` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.2%` | `STOP_LOSS_HIT` | $0.2588 |
| 2558 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:41:36 UTC | 37.0s | `1.604` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.4%` | `MIN_PROFIT_TP_HIT` | $0.2592 |
| 2559 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:01:35 UTC | 11m 35s | `1.607` | `1.605` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2596 |
| 2560 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:16:13 UTC | 7m 13s | `1.605` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2600 |
| 2561 | `SHORT` | 2026-07-23 23:19:59 UTC | 2026-07-23 23:47:35 UTC | 27m 35s | `1.606` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.3%` | `MIN_PROFIT_TP_HIT` | $0.2604 |
| 2562 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:06:03 UTC | 11m 03s | `1.599` | `1.591` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.5%` | `STOP_LOSS_HIT` | $0.2588 |

> 💡 *Full granular dataset with all 2562 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
