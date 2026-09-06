# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:15:49 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.2216 USDT` | `₹20.93` | `+216.57%` |
| **Net Realized PnL** | **`+0.1516 USDT`** | **`₹+14.32`** | **`+216.57% Net ROI`** |
| **Gross Profit** | `+0.6576 USDT` | `₹62.11` | Total positive trade returns |
| **Gross Loss** | `-0.5060 USDT` | `₹47.79` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.30`** | — | Profitable |
| **Win / Loss Payoff** | `0.40` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0164 USDT` | `₹1.55` | **`-8.29%` Peak-to-Trough** |
| **Win Rate** | **`76.47%`** | — | `1644 Wins / 506 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `10.20` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `6.15` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `26.12` | — | Net ROI divided by Max Drawdown |

---

## 🛠️ Complete Configuration & Settings Used

### Strategy & Market Setup
| Configuration Setting | Value | Operational Details |
| :--- | :--- | :--- |
| **Trading Pair Symbol** | `TRUMP_USDT` | Base Asset: `TRUMP` / Quote Asset: `USDT` |
| **Candle Timeframe** | `1m` | Dynamic candle granularity evaluated by strategy indicators |
| **Strategy Evaluated** | `STOCH_RSI` | Stochastic RSI Momentum Scalper (Preset: FAST_SCALP ; Overbought/Oversold Reversal) |
| **Strategy Preset** | `FAST_SCALP` | Configured indicator preset profile |
| **Evaluation Date Range** | `2026-07-25` → `2026-08-15` | Historical evaluation window |
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
| **Total Trades Executed** | `2150` | Total completed trade lifecycle events |
| **Winning Trades** | `1644` | `76.47%` of total trades |
| **Losing Trades** | `506` | `23.53%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0001 USDT` (`₹+0.01`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0010 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.6% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0010 USDT (-24.1% ROE)` | Trade #14 (SHORT) |
| **Max Consecutive Wins** | `33` trades | Peak winning streak |
| **Max Consecutive Losses** | `6` trades | Peak losing streak |
| **Average Trade Duration** | `8m 02s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.2s` | Trade #650 |
| **Longest Trade In-Position** | `1h 56m 40s` | Trade #1177 |
| **Cumulative Time In Position** | `288h 11m 01s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1086` (50.5%) | `1064` (49.5%) | `2150` |
| **Wins / Losses** | `810 W / 276 L` | `834 W / 230 L` | `1644 W / 506 L` |
| **Win Rate** | **`74.59%`** | **`78.38%`** | **`76.47%`** |
| **Gross Profit** | `+0.3240 USDT` | `+0.3336 USDT` | `+0.6576 USDT` |
| **Gross Loss** | `-0.2760 USDT` | `-0.2300 USDT` | `-0.5060 USDT` |
| **Net Realized PnL** | **`+0.0480 USDT`** | **`+0.1036 USDT`** | **`+0.1516 USDT`** |
| **Net PnL (INR)** | `₹+4.53` | `₹+9.79` | `₹+14.32` |
| **Profit Factor** | `1.17` | `1.45` | `1.30` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1644` | `76.5%` | `+0.6576 USDT` | `₹+62.11` | `100.0%` | `6m 19s` |
| `STOP_LOSS_HIT` | `506` | `23.5%` | `-0.5060 USDT` | `₹-47.79` | `0.0%` | `13m 36s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-25 00:27:59 UTC | 2026-07-25 00:31:24 UTC | 3m 24s | `1.561` | `1.563` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-07-25 00:36:59 UTC | 2026-07-25 00:42:01 UTC | 5m 01s | `1.563` | `1.561` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 3 | `LONG` | 2026-07-25 00:44:59 UTC | 2026-07-25 00:46:48 UTC | 1m 48s | `1.560` | `1.562` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 4 | `LONG` | 2026-07-25 00:47:59 UTC | 2026-07-25 00:58:14 UTC | 10m 14s | `1.564` | `1.566` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0716 |
| 5 | `SHORT` | 2026-07-25 01:00:59 UTC | 2026-07-25 01:04:37 UTC | 3m 37s | `1.567` | `1.565` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0720 |
| 6 | `LONG` | 2026-07-25 01:13:59 UTC | 2026-07-25 01:16:13 UTC | 2m 13s | `1.561` | `1.563` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0724 |
| 7 | `SHORT` | 2026-07-25 01:31:59 UTC | 2026-07-25 01:45:41 UTC | 13m 41s | `1.558` | `1.556` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0728 |
| 8 | `LONG` | 2026-07-25 01:56:59 UTC | 2026-07-25 01:57:54 UTC | 54.9s | `1.556` | `1.558` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0732 |
| 9 | `LONG` | 2026-07-25 02:04:59 UTC | 2026-07-25 02:06:42 UTC | 1m 42s | `1.552` | `1.554` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.7%` | `MIN_PROFIT_TP_HIT` | $0.0736 |
| 10 | `SHORT` | 2026-07-25 02:10:59 UTC | 2026-07-25 02:14:00 UTC | 3m 00s | `1.557` | `1.555` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0740 |
| 11 | `LONG` | 2026-07-25 02:19:59 UTC | 2026-07-25 02:39:46 UTC | 19m 46s | `1.556` | `1.558` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0744 |
| 12 | `SHORT` | 2026-07-25 02:45:59 UTC | 2026-07-25 02:48:47 UTC | 2m 47s | `1.558` | `1.556` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0748 |
| 13 | `LONG` | 2026-07-25 02:51:59 UTC | 2026-07-25 02:52:49 UTC | 49.1s | `1.555` | `1.557` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0752 |
| 14 | `SHORT` | 2026-07-25 02:57:59 UTC | 2026-07-25 03:05:49 UTC | 7m 49s | `1.559` | `1.564` | $0.31 | $0.00 | $0.000000 | **-0.0010** | `-24.1%` | `STOP_LOSS_HIT` | $0.0742 |
| 15 | `SHORT` | 2026-07-25 03:11:59 UTC | 2026-07-25 03:13:40 UTC | 1m 40s | `1.566` | `1.571` | $0.31 | $0.00 | $0.000000 | **-0.0010** | `-23.9%` | `STOP_LOSS_HIT` | $0.0732 |
| 16 | `LONG` | 2026-07-25 03:22:59 UTC | 2026-07-25 03:26:01 UTC | 3m 01s | `1.569` | `1.571` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0736 |
| 17 | `LONG` | 2026-07-25 03:34:59 UTC | 2026-07-25 03:47:36 UTC | 12m 36s | `1.570` | `1.565` | $0.31 | $0.00 | $0.000000 | **-0.0010** | `-23.9%` | `STOP_LOSS_HIT` | $0.0726 |
| 18 | `LONG` | 2026-07-25 03:52:59 UTC | 2026-07-25 03:57:14 UTC | 4m 14s | `1.565` | `1.567` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0730 |
| 19 | `SHORT` | 2026-07-25 03:59:59 UTC | 2026-07-25 04:12:18 UTC | 12m 18s | `1.566` | `1.571` | $0.31 | $0.00 | $0.000000 | **-0.0010** | `-23.9%` | `STOP_LOSS_HIT` | $0.0720 |
| 20 | `SHORT` | 2026-07-25 04:20:59 UTC | 2026-07-25 05:07:01 UTC | 46m 01s | `1.574` | `1.572` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.5%` | `MIN_PROFIT_TP_HIT` | $0.0724 |
| 21 | `LONG` | 2026-07-25 05:10:59 UTC | 2026-07-25 05:13:25 UTC | 2m 25s | `1.573` | `1.568` | $0.31 | $0.00 | $0.000000 | **-0.0010** | `-23.8%` | `STOP_LOSS_HIT` | $0.0714 |
| 22 | `LONG` | 2026-07-25 05:19:59 UTC | 2026-07-25 05:21:48 UTC | 1m 48s | `1.566` | `1.568` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0718 |
| 23 | `SHORT` | 2026-07-25 05:26:59 UTC | 2026-07-25 05:35:15 UTC | 8m 15s | `1.567` | `1.565` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0722 |
| 24 | `SHORT` | 2026-07-25 05:59:59 UTC | 2026-07-25 06:10:09 UTC | 10m 09s | `1.564` | `1.562` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0726 |
| 25 | `LONG` | 2026-07-25 06:12:59 UTC | 2026-07-25 06:18:49 UTC | 5m 49s | `1.563` | `1.565` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0730 |
| ... | ... | *(2100 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2126 | `LONG` | 2026-08-14 20:16:59 UTC | 2026-08-14 20:17:05 UTC | 5.6s | `1.445` | `1.447` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.4%` | `MIN_PROFIT_TP_HIT` | $0.2176 |
| 2127 | `LONG` | 2026-08-14 20:25:59 UTC | 2026-08-14 20:27:51 UTC | 1m 51s | `1.445` | `1.447` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.4%` | `MIN_PROFIT_TP_HIT` | $0.2180 |
| 2128 | `LONG` | 2026-08-14 20:37:59 UTC | 2026-08-14 20:38:47 UTC | 47.6s | `1.448` | `1.450` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.4%` | `MIN_PROFIT_TP_HIT` | $0.2184 |
| 2129 | `SHORT` | 2026-08-14 20:44:59 UTC | 2026-08-14 20:45:18 UTC | 19.0s | `1.452` | `1.450` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.3%` | `MIN_PROFIT_TP_HIT` | $0.2188 |
| 2130 | `LONG` | 2026-08-14 20:49:59 UTC | 2026-08-14 20:53:26 UTC | 3m 26s | `1.454` | `1.449` | $0.29 | $0.00 | $0.000000 | **-0.0010** | `-25.8%` | `STOP_LOSS_HIT` | $0.2178 |
| 2131 | `LONG` | 2026-08-14 20:59:59 UTC | 2026-08-14 21:01:36 UTC | 1m 36s | `1.451` | `1.453` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.3%` | `MIN_PROFIT_TP_HIT` | $0.2182 |
| 2132 | `SHORT` | 2026-08-14 21:04:59 UTC | 2026-08-14 21:08:35 UTC | 3m 35s | `1.447` | `1.445` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.4%` | `MIN_PROFIT_TP_HIT` | $0.2186 |
| 2133 | `LONG` | 2026-08-14 21:12:59 UTC | 2026-08-14 21:18:46 UTC | 5m 46s | `1.448` | `1.443` | $0.29 | $0.00 | $0.000000 | **-0.0010** | `-25.9%` | `STOP_LOSS_HIT` | $0.2176 |
| 2134 | `LONG` | 2026-08-14 21:23:59 UTC | 2026-08-14 21:27:39 UTC | 3m 39s | `1.437` | `1.439` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.4%` | `MIN_PROFIT_TP_HIT` | $0.2180 |
| 2135 | `SHORT` | 2026-08-14 21:31:59 UTC | 2026-08-14 21:33:36 UTC | 1m 36s | `1.438` | `1.436` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.4%` | `MIN_PROFIT_TP_HIT` | $0.2184 |
| 2136 | `LONG` | 2026-08-14 21:42:59 UTC | 2026-08-14 21:50:07 UTC | 7m 07s | `1.431` | `1.433` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.2188 |
| 2137 | `SHORT` | 2026-08-14 21:53:59 UTC | 2026-08-14 21:54:26 UTC | 26.1s | `1.428` | `1.426` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.2192 |
| 2138 | `LONG` | 2026-08-14 21:58:59 UTC | 2026-08-14 22:01:27 UTC | 2m 27s | `1.430` | `1.432` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.2196 |
| 2139 | `SHORT` | 2026-08-14 22:05:59 UTC | 2026-08-14 22:06:40 UTC | 40.9s | `1.430` | `1.428` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.2200 |
| 2140 | `LONG` | 2026-08-14 22:10:59 UTC | 2026-08-14 22:12:05 UTC | 1m 05s | `1.429` | `1.431` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.2204 |
| 2141 | `LONG` | 2026-08-14 22:22:59 UTC | 2026-08-14 22:29:16 UTC | 6m 16s | `1.423` | `1.418` | $0.28 | $0.00 | $0.000000 | **-0.0010** | `-26.4%` | `STOP_LOSS_HIT` | $0.2194 |
| 2142 | `SHORT` | 2026-08-14 22:38:59 UTC | 2026-08-14 22:45:03 UTC | 6m 03s | `1.422` | `1.420` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.2198 |
| 2143 | `LONG` | 2026-08-14 22:47:59 UTC | 2026-08-14 23:01:43 UTC | 13m 43s | `1.423` | `1.425` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.2202 |
| 2144 | `SHORT` | 2026-08-14 23:03:59 UTC | 2026-08-14 23:08:38 UTC | 4m 38s | `1.424` | `1.422` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.2206 |
| 2145 | `LONG` | 2026-08-14 23:11:59 UTC | 2026-08-14 23:15:10 UTC | 3m 10s | `1.424` | `1.426` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.2210 |
| 2146 | `SHORT` | 2026-08-14 23:18:59 UTC | 2026-08-14 23:26:51 UTC | 7m 51s | `1.426` | `1.431` | $0.29 | $0.00 | $0.000000 | **-0.0010** | `-26.3%` | `STOP_LOSS_HIT` | $0.2200 |
| 2147 | `SHORT` | 2026-08-14 23:28:59 UTC | 2026-08-14 23:30:03 UTC | 1m 03s | `1.429` | `1.427` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.2204 |
| 2148 | `LONG` | 2026-08-14 23:34:59 UTC | 2026-08-14 23:37:33 UTC | 2m 33s | `1.427` | `1.429` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.2208 |
| 2149 | `SHORT` | 2026-08-14 23:44:59 UTC | 2026-08-14 23:51:47 UTC | 6m 47s | `1.433` | `1.431` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.2212 |
| 2150 | `LONG` | 2026-08-14 23:52:59 UTC | 2026-08-15 00:01:28 UTC | 8m 28s | `1.433` | `1.435` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.2216 |

> 💡 *Full granular dataset with all 2150 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
