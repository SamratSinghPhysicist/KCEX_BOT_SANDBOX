# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:17:38 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.1756 USDT` | `₹16.59` | `+150.86%` |
| **Net Realized PnL** | **`+0.1056 USDT`** | **`₹+9.97`** | **`+150.86% Net ROI`** |
| **Gross Profit** | `+0.8232 USDT` | `₹77.75` | Total positive trade returns |
| **Gross Loss** | `-0.7176 USDT` | `₹67.78` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.15`** | — | Profitable |
| **Win / Loss Payoff** | `0.27` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0176 USDT` | `₹1.66` | **`-12.32%` Peak-to-Trough** |
| **Win Rate** | **`80.74%`** | — | `2058 Wins / 491 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `5.19` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `2.65` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `12.24` | — | Net ROI divided by Max Drawdown |

---

## 🛠️ Complete Configuration & Settings Used

### Strategy & Market Setup
| Configuration Setting | Value | Operational Details |
| :--- | :--- | :--- |
| **Trading Pair Symbol** | `TRUMP_USDT` | Base Asset: `TRUMP` / Quote Asset: `USDT` |
| **Candle Timeframe** | `1m` | Dynamic candle granularity evaluated by strategy indicators |
| **Strategy Evaluated** | `STOCH_RSI` | Stochastic RSI Momentum Scalper (Preset: FAST_SCALP ; Overbought/Oversold Reversal) |
| **Strategy Preset** | `FAST_SCALP` | Configured indicator preset profile |
| **Evaluation Date Range** | `2026-08-16` → `2026-08-31` | Historical evaluation window |
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
| **Stop Loss Rule** | `-25.0% ROE on committed margin` | Stop loss evaluation logic |

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
| **Total Trades Executed** | `2549` | Total completed trade lifecycle events |
| **Winning Trades** | `2058` | `80.74%` of total trades |
| **Losing Trades** | `491` | `19.26%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0015 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+7.3% ROE)` | Trade #783 (SHORT) |
| **Largest Losing Trade** | `-0.0022 USDT (-25.7% ROE)` | Trade #808 (SHORT) |
| **Max Consecutive Wins** | `27` trades | Peak winning streak |
| **Max Consecutive Losses** | `5` trades | Peak losing streak |
| **Average Trade Duration** | `1m 52s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #360 |
| **Longest Trade In-Position** | `1h 26m 07s` | Trade #131 |
| **Cumulative Time In Position** | `79h 41m 01s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1306` (51.2%) | `1243` (48.8%) | `2549` |
| **Wins / Losses** | `1044 W / 262 L` | `1014 W / 229 L` | `2058 W / 491 L` |
| **Win Rate** | **`79.94%`** | **`81.58%`** | **`80.74%`** |
| **Gross Profit** | `+0.4176 USDT` | `+0.4056 USDT` | `+0.8232 USDT` |
| **Gross Loss** | `-0.3904 USDT` | `-0.3272 USDT` | `-0.7176 USDT` |
| **Net Realized PnL** | **`+0.0272 USDT`** | **`+0.0784 USDT`** | **`+0.1056 USDT`** |
| **Net PnL (INR)** | `₹+2.57` | `₹+7.40` | `₹+9.97` |
| **Profit Factor** | `1.07` | `1.24` | `1.15` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `2058` | `80.7%` | `+0.8232 USDT` | `₹+77.75` | `100.0%` | `1m 26s` |
| `STOP_LOSS_HIT` | `491` | `19.3%` | `-0.7176 USDT` | `₹-67.78` | `0.0%` | `3m 41s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-08-16 00:26:59 UTC | 2026-08-16 00:27:20 UTC | 20.3s | `1.409` | `1.411` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.6%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-08-16 00:31:59 UTC | 2026-08-16 00:40:07 UTC | 8m 07s | `1.410` | `1.408` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.6%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 3 | `LONG` | 2026-08-16 00:44:59 UTC | 2026-08-16 00:53:26 UTC | 8m 26s | `1.408` | `1.410` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 4 | `SHORT` | 2026-08-16 00:56:59 UTC | 2026-08-16 01:09:02 UTC | 12m 02s | `1.410` | `1.408` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.6%` | `MIN_PROFIT_TP_HIT` | $0.0716 |
| 5 | `LONG` | 2026-08-16 01:17:59 UTC | 2026-08-16 01:18:48 UTC | 48.9s | `1.403` | `1.405` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0720 |
| 6 | `SHORT` | 2026-08-16 01:22:59 UTC | 2026-08-16 01:26:18 UTC | 3m 18s | `1.402` | `1.400` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0724 |
| 7 | `LONG` | 2026-08-16 01:32:59 UTC | 2026-08-16 01:33:06 UTC | 6.9s | `1.393` | `1.395` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0728 |
| 8 | `SHORT` | 2026-08-16 01:38:59 UTC | 2026-08-16 01:45:48 UTC | 6m 48s | `1.392` | `1.397` | $0.28 | $0.00 | $0.000000 | **-0.0010** | `-26.9%` | `STOP_LOSS_HIT` | $0.0718 |
| 9 | `SHORT` | 2026-08-16 01:47:59 UTC | 2026-08-16 01:53:49 UTC | 5m 49s | `1.395` | `1.393` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0722 |
| 10 | `LONG` | 2026-08-16 01:59:59 UTC | 2026-08-16 02:13:06 UTC | 13m 06s | `1.395` | `1.390` | $0.28 | $0.00 | $0.000000 | **-0.0010** | `-26.9%` | `STOP_LOSS_HIT` | $0.0712 |
| 11 | `LONG` | 2026-08-16 02:16:59 UTC | 2026-08-16 02:20:11 UTC | 3m 11s | `1.390` | `1.392` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0716 |
| 12 | `SHORT` | 2026-08-16 02:29:59 UTC | 2026-08-16 02:45:38 UTC | 15m 38s | `1.395` | `1.393` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0720 |
| 13 | `LONG` | 2026-08-16 02:48:59 UTC | 2026-08-16 03:04:39 UTC | 15m 39s | `1.393` | `1.395` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0724 |
| 14 | `SHORT` | 2026-08-16 03:08:59 UTC | 2026-08-16 03:13:43 UTC | 4m 43s | `1.394` | `1.392` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0728 |
| 15 | `LONG` | 2026-08-16 03:17:59 UTC | 2026-08-16 03:26:22 UTC | 8m 22s | `1.393` | `1.395` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0732 |
| 16 | `SHORT` | 2026-08-16 03:36:59 UTC | 2026-08-16 03:52:02 UTC | 15m 02s | `1.395` | `1.393` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0736 |
| 17 | `LONG` | 2026-08-16 03:56:59 UTC | 2026-08-16 04:17:06 UTC | 20m 06s | `1.394` | `1.389` | $0.28 | $0.00 | $0.000000 | **-0.0010** | `-26.9%` | `STOP_LOSS_HIT` | $0.0726 |
| 18 | `SHORT` | 2026-08-16 04:23:59 UTC | 2026-08-16 04:38:06 UTC | 14m 06s | `1.392` | `1.397` | $0.28 | $0.00 | $0.000000 | **-0.0010** | `-26.9%` | `STOP_LOSS_HIT` | $0.0716 |
| 19 | `SHORT` | 2026-08-16 04:42:59 UTC | 2026-08-16 04:56:49 UTC | 13m 49s | `1.399` | `1.397` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0720 |
| 20 | `LONG` | 2026-08-16 05:00:59 UTC | 2026-08-16 05:02:20 UTC | 1m 20s | `1.397` | `1.399` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0724 |
| 21 | `SHORT` | 2026-08-16 05:06:59 UTC | 2026-08-16 05:18:43 UTC | 11m 43s | `1.398` | `1.396` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0728 |
| 22 | `LONG` | 2026-08-16 05:20:59 UTC | 2026-08-16 05:36:28 UTC | 15m 28s | `1.397` | `1.399` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0732 |
| 23 | `SHORT` | 2026-08-16 05:39:59 UTC | 2026-08-16 05:43:58 UTC | 3m 58s | `1.399` | `1.397` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0736 |
| 24 | `LONG` | 2026-08-16 05:47:59 UTC | 2026-08-16 06:14:37 UTC | 26m 37s | `1.399` | `1.394` | $0.28 | $0.00 | $0.000000 | **-0.0010** | `-26.8%` | `STOP_LOSS_HIT` | $0.0726 |
| 25 | `LONG` | 2026-08-16 06:19:59 UTC | 2026-08-16 06:26:00 UTC | 6m 00s | `1.393` | `1.395` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0730 |
| ... | ... | *(2499 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2525 | `SHORT` | 2026-08-30 20:40:59 UTC | 2026-08-30 20:42:10 UTC | 1m 10s | `2.514` | `2.512` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1720 |
| 2526 | `LONG` | 2026-08-30 20:46:59 UTC | 2026-08-30 20:47:10 UTC | 10.1s | `2.518` | `2.520` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1724 |
| 2527 | `SHORT` | 2026-08-30 20:50:59 UTC | 2026-08-30 20:52:17 UTC | 1m 17s | `2.525` | `2.523` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.1728 |
| 2528 | `SHORT` | 2026-08-30 20:54:59 UTC | 2026-08-30 20:56:30 UTC | 1m 30s | `2.525` | `2.523` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.1732 |
| 2529 | `LONG` | 2026-08-30 21:03:59 UTC | 2026-08-30 21:04:03 UTC | 3.9s | `2.500` | `2.502` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1736 |
| 2530 | `SHORT` | 2026-08-30 21:15:59 UTC | 2026-08-30 21:16:07 UTC | 7.4s | `2.503` | `2.501` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1740 |
| 2531 | `SHORT` | 2026-08-30 21:32:59 UTC | 2026-08-30 21:33:09 UTC | 9.9s | `2.509` | `2.507` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1744 |
| 2532 | `SHORT` | 2026-08-30 21:35:59 UTC | 2026-08-30 21:37:12 UTC | 1m 12s | `2.510` | `2.508` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1748 |
| 2533 | `LONG` | 2026-08-30 21:50:59 UTC | 2026-08-30 21:51:00 UTC | 0.5s | `2.488` | `2.490` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1752 |
| 2534 | `SHORT` | 2026-08-30 21:58:59 UTC | 2026-08-30 22:00:04 UTC | 1m 04s | `2.506` | `2.504` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1756 |
| 2535 | `LONG` | 2026-08-30 22:09:59 UTC | 2026-08-30 22:10:03 UTC | 3.7s | `2.516` | `2.518` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1760 |
| 2536 | `LONG` | 2026-08-30 22:19:59 UTC | 2026-08-30 22:21:27 UTC | 1m 27s | `2.501` | `2.493` | $0.50 | $0.01 | $0.000000 | **-0.0016** | `-24.0%` | `STOP_LOSS_HIT` | $0.1744 |
| 2537 | `SHORT` | 2026-08-30 22:43:59 UTC | 2026-08-30 22:44:04 UTC | 4.8s | `2.429` | `2.427` | $0.49 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1748 |
| 2538 | `LONG` | 2026-08-30 22:51:59 UTC | 2026-08-30 22:52:04 UTC | 4.7s | `2.416` | `2.418` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1752 |
| 2539 | `SHORT` | 2026-08-30 22:56:59 UTC | 2026-08-30 22:59:02 UTC | 2m 02s | `2.424` | `2.422` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1756 |
| 2540 | `SHORT` | 2026-08-30 23:00:59 UTC | 2026-08-30 23:01:39 UTC | 39.8s | `2.409` | `2.417` | $0.48 | $0.01 | $0.000000 | **-0.0016** | `-24.9%` | `STOP_LOSS_HIT` | $0.1740 |
| 2541 | `SHORT` | 2026-08-30 23:10:59 UTC | 2026-08-30 23:11:23 UTC | 23.0s | `2.405` | `2.413` | $0.48 | $0.01 | $0.000000 | **-0.0016** | `-24.9%` | `STOP_LOSS_HIT` | $0.1724 |
| 2542 | `SHORT` | 2026-08-30 23:15:59 UTC | 2026-08-30 23:16:00 UTC | 0.8s | `2.422` | `2.420` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1728 |
| 2543 | `SHORT` | 2026-08-30 23:18:59 UTC | 2026-08-30 23:19:00 UTC | 0.6s | `2.415` | `2.413` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1732 |
| 2544 | `SHORT` | 2026-08-30 23:24:59 UTC | 2026-08-30 23:25:00 UTC | 0.6s | `2.414` | `2.412` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1736 |
| 2545 | `LONG` | 2026-08-30 23:32:59 UTC | 2026-08-30 23:33:01 UTC | 1.6s | `2.388` | `2.390` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.3%` | `MIN_PROFIT_TP_HIT` | $0.1740 |
| 2546 | `LONG` | 2026-08-30 23:42:59 UTC | 2026-08-30 23:43:19 UTC | 19.7s | `2.330` | `2.332` | $0.47 | $0.01 | $0.000000 | **+0.0004** | `+6.4%` | `MIN_PROFIT_TP_HIT` | $0.1744 |
| 2547 | `SHORT` | 2026-08-30 23:53:59 UTC | 2026-08-30 23:54:11 UTC | 11.8s | `2.330` | `2.328` | $0.47 | $0.01 | $0.000000 | **+0.0004** | `+6.4%` | `MIN_PROFIT_TP_HIT` | $0.1748 |
| 2548 | `SHORT` | 2026-08-30 23:57:59 UTC | 2026-08-30 23:58:00 UTC | 0.5s | `2.343` | `2.341` | $0.47 | $0.01 | $0.000000 | **+0.0004** | `+6.4%` | `MIN_PROFIT_TP_HIT` | $0.1752 |
| 2549 | `SHORT` | 2026-08-31 00:00:59 UTC | 2026-08-31 00:01:02 UTC | 2.0s | `2.338` | `2.336` | $0.47 | $0.01 | $0.000000 | **+0.0004** | `+6.4%` | `MIN_PROFIT_TP_HIT` | $0.1756 |

> 💡 *Full granular dataset with all 2549 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
