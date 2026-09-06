# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:17:22 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.1702 USDT` | `₹16.08` | `+143.14%` |
| **Net Realized PnL** | **`+0.1002 USDT`** | **`₹+9.46`** | **`+143.14% Net ROI`** |
| **Gross Profit** | `+0.7652 USDT` | `₹72.27` | Total positive trade returns |
| **Gross Loss** | `-0.6650 USDT` | `₹62.81` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.15`** | — | Profitable |
| **Win / Loss Payoff** | `0.40` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0148 USDT` | `₹1.40` | **`-9.23%` Peak-to-Trough** |
| **Win Rate** | **`74.20%`** | — | `1913 Wins / 665 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `5.51` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `3.40` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `15.50` | — | Net ROI divided by Max Drawdown |

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
| **Total Trades Executed** | `2578` | Total completed trade lifecycle events |
| **Winning Trades** | `1913` | `74.20%` of total trades |
| **Losing Trades** | `665` | `25.80%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0010 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+7.3% ROE)` | Trade #790 (SHORT) |
| **Largest Losing Trade** | `-0.0010 USDT (-17.0% ROE)` | Trade #796 (LONG) |
| **Max Consecutive Wins** | `19` trades | Peak winning streak |
| **Max Consecutive Losses** | `5` trades | Peak losing streak |
| **Average Trade Duration** | `1m 41s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #360 |
| **Longest Trade In-Position** | `1h 26m 07s` | Trade #131 |
| **Cumulative Time In Position** | `72h 53m 29s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1319` (51.2%) | `1259` (48.8%) | `2578` |
| **Wins / Losses** | `974 W / 345 L` | `939 W / 320 L` | `1913 W / 665 L` |
| **Win Rate** | **`73.84%`** | **`74.58%`** | **`74.20%`** |
| **Gross Profit** | `+0.3896 USDT` | `+0.3756 USDT` | `+0.7652 USDT` |
| **Gross Loss** | `-0.3450 USDT` | `-0.3200 USDT` | `-0.6650 USDT` |
| **Net Realized PnL** | **`+0.0446 USDT`** | **`+0.0556 USDT`** | **`+0.1002 USDT`** |
| **Net PnL (INR)** | `₹+4.21` | `₹+5.25` | `₹+9.46` |
| **Profit Factor** | `1.13` | `1.17` | `1.15` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1913` | `74.2%` | `+0.7652 USDT` | `₹+72.27` | `100.0%` | `1m 24s` |
| `STOP_LOSS_HIT` | `665` | `25.8%` | `-0.6650 USDT` | `₹-62.81` | `0.0%` | `2m 30s` |

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
| ... | ... | *(2528 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2554 | `SHORT` | 2026-08-30 20:40:59 UTC | 2026-08-30 20:41:52 UTC | 52.8s | `2.514` | `2.519` | $0.50 | $0.01 | $0.000000 | **-0.0010** | `-14.9%` | `STOP_LOSS_HIT` | $0.1676 |
| 2555 | `LONG` | 2026-08-30 20:46:59 UTC | 2026-08-30 20:47:10 UTC | 10.1s | `2.518` | `2.520` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1680 |
| 2556 | `SHORT` | 2026-08-30 20:50:59 UTC | 2026-08-30 20:52:17 UTC | 1m 17s | `2.525` | `2.523` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.1684 |
| 2557 | `SHORT` | 2026-08-30 20:54:59 UTC | 2026-08-30 20:56:30 UTC | 1m 30s | `2.525` | `2.523` | $0.51 | $0.01 | $0.000000 | **+0.0004** | `+5.9%` | `MIN_PROFIT_TP_HIT` | $0.1688 |
| 2558 | `LONG` | 2026-08-30 21:03:59 UTC | 2026-08-30 21:04:03 UTC | 3.9s | `2.500` | `2.502` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1692 |
| 2559 | `SHORT` | 2026-08-30 21:15:59 UTC | 2026-08-30 21:16:07 UTC | 7.4s | `2.503` | `2.501` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1696 |
| 2560 | `SHORT` | 2026-08-30 21:32:59 UTC | 2026-08-30 21:33:09 UTC | 9.9s | `2.509` | `2.507` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1700 |
| 2561 | `SHORT` | 2026-08-30 21:35:59 UTC | 2026-08-30 21:37:12 UTC | 1m 12s | `2.510` | `2.508` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1704 |
| 2562 | `LONG` | 2026-08-30 21:50:59 UTC | 2026-08-30 21:51:00 UTC | 0.5s | `2.488` | `2.490` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1708 |
| 2563 | `SHORT` | 2026-08-30 21:58:59 UTC | 2026-08-30 21:59:58 UTC | 58.1s | `2.506` | `2.511` | $0.50 | $0.01 | $0.000000 | **-0.0010** | `-15.0%` | `STOP_LOSS_HIT` | $0.1698 |
| 2564 | `LONG` | 2026-08-30 22:09:59 UTC | 2026-08-30 22:10:03 UTC | 3.7s | `2.516` | `2.518` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1702 |
| 2565 | `LONG` | 2026-08-30 22:19:59 UTC | 2026-08-30 22:21:17 UTC | 1m 17s | `2.501` | `2.496` | $0.50 | $0.01 | $0.000000 | **-0.0010** | `-15.0%` | `STOP_LOSS_HIT` | $0.1692 |
| 2566 | `SHORT` | 2026-08-30 22:43:59 UTC | 2026-08-30 22:44:04 UTC | 4.8s | `2.429` | `2.427` | $0.49 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1696 |
| 2567 | `LONG` | 2026-08-30 22:51:59 UTC | 2026-08-30 22:52:04 UTC | 4.7s | `2.416` | `2.418` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1700 |
| 2568 | `SHORT` | 2026-08-30 22:56:59 UTC | 2026-08-30 22:59:02 UTC | 2m 02s | `2.424` | `2.422` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1704 |
| 2569 | `SHORT` | 2026-08-30 23:00:59 UTC | 2026-08-30 23:01:05 UTC | 5.0s | `2.409` | `2.414` | $0.48 | $0.01 | $0.000000 | **-0.0010** | `-15.6%` | `STOP_LOSS_HIT` | $0.1694 |
| 2570 | `SHORT` | 2026-08-30 23:10:59 UTC | 2026-08-30 23:11:14 UTC | 14.9s | `2.405` | `2.410` | $0.48 | $0.01 | $0.000000 | **-0.0010** | `-15.6%` | `STOP_LOSS_HIT` | $0.1684 |
| 2571 | `SHORT` | 2026-08-30 23:15:59 UTC | 2026-08-30 23:16:00 UTC | 0.8s | `2.422` | `2.420` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1688 |
| 2572 | `SHORT` | 2026-08-30 23:18:59 UTC | 2026-08-30 23:19:00 UTC | 0.6s | `2.415` | `2.413` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1692 |
| 2573 | `SHORT` | 2026-08-30 23:24:59 UTC | 2026-08-30 23:25:00 UTC | 0.6s | `2.414` | `2.412` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1696 |
| 2574 | `LONG` | 2026-08-30 23:32:59 UTC | 2026-08-30 23:33:01 UTC | 1.6s | `2.388` | `2.390` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.3%` | `MIN_PROFIT_TP_HIT` | $0.1700 |
| 2575 | `LONG` | 2026-08-30 23:42:59 UTC | 2026-08-30 23:43:06 UTC | 6.5s | `2.330` | `2.325` | $0.47 | $0.01 | $0.000000 | **-0.0010** | `-16.1%` | `STOP_LOSS_HIT` | $0.1690 |
| 2576 | `SHORT` | 2026-08-30 23:53:59 UTC | 2026-08-30 23:54:11 UTC | 11.8s | `2.330` | `2.328` | $0.47 | $0.01 | $0.000000 | **+0.0004** | `+6.4%` | `MIN_PROFIT_TP_HIT` | $0.1694 |
| 2577 | `SHORT` | 2026-08-30 23:57:59 UTC | 2026-08-30 23:58:00 UTC | 0.5s | `2.343` | `2.341` | $0.47 | $0.01 | $0.000000 | **+0.0004** | `+6.4%` | `MIN_PROFIT_TP_HIT` | $0.1698 |
| 2578 | `SHORT` | 2026-08-31 00:00:59 UTC | 2026-08-31 00:01:02 UTC | 2.0s | `2.338` | `2.336` | $0.47 | $0.01 | $0.000000 | **+0.0004** | `+6.4%` | `MIN_PROFIT_TP_HIT` | $0.1702 |

> 💡 *Full granular dataset with all 2578 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
