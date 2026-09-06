# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:16:33 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.0928 USDT` | `₹8.76` | `+32.57%` |
| **Net Realized PnL** | **`+0.0228 USDT`** | **`₹+2.15`** | **`+32.57% Net ROI`** |
| **Gross Profit** | `+0.3748 USDT` | `₹35.40` | Total positive trade returns |
| **Gross Loss** | `-0.3520 USDT` | `₹33.25` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.06`** | — | Profitable |
| **Win / Loss Payoff** | `0.40` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0194 USDT` | `₹1.83` | **`-17.51%` Peak-to-Trough** |
| **Win Rate** | **`72.69%`** | — | `937 Wins / 352 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `2.73` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `1.71` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `1.86` | — | Net ROI divided by Max Drawdown |

---

## 🛠️ Complete Configuration & Settings Used

### Strategy & Market Setup
| Configuration Setting | Value | Operational Details |
| :--- | :--- | :--- |
| **Trading Pair Symbol** | `TRUMP_USDT` | Base Asset: `TRUMP` / Quote Asset: `USDT` |
| **Candle Timeframe** | `1m` | Dynamic candle granularity evaluated by strategy indicators |
| **Strategy Evaluated** | `EMA_CROSSOVER` | EMA Crossover Trend Follower (Preset: 5/13 ; Closed Candle Confirmation: True) |
| **Strategy Preset** | `5/13` | Configured indicator preset profile |
| **Evaluation Date Range** | `2026-07-25` → `2026-08-15` | Historical evaluation window |
| **High-Fidelity Simulation** | `ENABLED (Tick Trades)` | Millisecond-level trade order matching & stop triggering |
| **Slippage Tolerance** | `0 ticks` (`0.000 USDT` per fill) | Adverse fill penalty applied to entry and exit orders |

### Strategy & Indicator Hyperparameters
| Hyperparameter | Value | Technical Context |
| :--- | :--- | :--- |
| **Active Strategy Engine** | `EMA_CROSSOVER` | Quantitative model evaluated |
| **Active Strategy Preset** | `5/13` | Selected preset configuration |
| **Fast EMA Period** | `5` | Short-term fast moving average |
| **Slow EMA Period** | `13` | Baseline slow moving average |
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
| **Total Trades Executed** | `1289` | Total completed trade lifecycle events |
| **Winning Trades** | `937` | `72.69%` of total trades |
| **Losing Trades** | `352` | `27.31%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0010 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.6% ROE)` | Trade #1 (SHORT) |
| **Largest Losing Trade** | `-0.0010 USDT (-23.8% ROE)` | Trade #12 (LONG) |
| **Max Consecutive Wins** | `18` trades | Peak winning streak |
| **Max Consecutive Losses** | `6` trades | Peak losing streak |
| **Average Trade Duration** | `9m 11s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #840 |
| **Longest Trade In-Position** | `1h 54m 25s` | Trade #1216 |
| **Cumulative Time In Position** | `197h 30m 49s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `650` (50.4%) | `639` (49.6%) | `1289` |
| **Wins / Losses** | `465 W / 185 L` | `472 W / 167 L` | `937 W / 352 L` |
| **Win Rate** | **`71.54%`** | **`73.87%`** | **`72.69%`** |
| **Gross Profit** | `+0.1860 USDT` | `+0.1888 USDT` | `+0.3748 USDT` |
| **Gross Loss** | `-0.1850 USDT` | `-0.1670 USDT` | `-0.3520 USDT` |
| **Net Realized PnL** | **`+0.0010 USDT`** | **`+0.0218 USDT`** | **`+0.0228 USDT`** |
| **Net PnL (INR)** | `₹+0.09` | `₹+2.06` | `₹+2.15` |
| **Profit Factor** | `1.01` | `1.13` | `1.06` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `937` | `72.7%` | `+0.3748 USDT` | `₹+35.40` | `100.0%` | `7m 13s` |
| `STOP_LOSS_HIT` | `352` | `27.3%` | `-0.3520 USDT` | `₹-33.25` | `0.0%` | `14m 25s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `SHORT` | 2026-07-25 00:21:59 UTC | 2026-07-25 00:43:24 UTC | 21m 24s | `1.562` | `1.560` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-07-25 00:44:59 UTC | 2026-07-25 00:56:45 UTC | 11m 45s | `1.560` | `1.565` | $0.31 | $0.00 | $0.000000 | **-0.0010** | `-24.0%` | `STOP_LOSS_HIT` | $0.0694 |
| 3 | `LONG` | 2026-07-25 00:57:59 UTC | 2026-07-25 01:00:01 UTC | 2m 01s | `1.565` | `1.567` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0698 |
| 4 | `SHORT` | 2026-07-25 01:09:59 UTC | 2026-07-25 01:11:49 UTC | 1m 49s | `1.562` | `1.560` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0702 |
| 5 | `LONG` | 2026-07-25 02:07:59 UTC | 2026-07-25 02:09:18 UTC | 1m 18s | `1.558` | `1.560` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0706 |
| 6 | `SHORT` | 2026-07-25 02:18:59 UTC | 2026-07-25 02:22:43 UTC | 3m 43s | `1.556` | `1.554` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0710 |
| 7 | `LONG` | 2026-07-25 02:29:59 UTC | 2026-07-25 02:39:46 UTC | 9m 46s | `1.556` | `1.558` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0714 |
| 8 | `SHORT` | 2026-07-25 02:49:59 UTC | 2026-07-25 02:57:32 UTC | 7m 32s | `1.556` | `1.561` | $0.31 | $0.00 | $0.000000 | **-0.0010** | `-24.1%` | `STOP_LOSS_HIT` | $0.0704 |
| 9 | `SHORT` | 2026-07-25 03:33:59 UTC | 2026-07-25 03:38:16 UTC | 4m 16s | `1.570` | `1.568` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 10 | `LONG` | 2026-07-25 03:44:59 UTC | 2026-07-25 04:04:14 UTC | 19m 14s | `1.567` | `1.569` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 11 | `SHORT` | 2026-07-25 04:51:59 UTC | 2026-07-25 04:52:23 UTC | 23.3s | `1.575` | `1.573` | $0.32 | $0.00 | $0.000000 | **+0.0004** | `+9.5%` | `MIN_PROFIT_TP_HIT` | $0.0716 |
| 12 | `LONG` | 2026-07-25 05:00:59 UTC | 2026-07-25 05:07:06 UTC | 6m 06s | `1.576` | `1.571` | $0.32 | $0.00 | $0.000000 | **-0.0010** | `-23.8%` | `STOP_LOSS_HIT` | $0.0706 |
| 13 | `LONG` | 2026-07-25 05:34:59 UTC | 2026-07-25 05:52:58 UTC | 17m 58s | `1.567` | `1.562` | $0.31 | $0.00 | $0.000000 | **-0.0010** | `-23.9%` | `STOP_LOSS_HIT` | $0.0696 |
| 14 | `LONG` | 2026-07-25 05:56:59 UTC | 2026-07-25 06:23:10 UTC | 26m 10s | `1.565` | `1.560` | $0.31 | $0.00 | $0.000000 | **-0.0010** | `-24.0%` | `STOP_LOSS_HIT` | $0.0686 |
| 15 | `LONG` | 2026-07-25 06:40:59 UTC | 2026-07-25 06:46:19 UTC | 5m 19s | `1.561` | `1.556` | $0.31 | $0.00 | $0.000000 | **-0.0010** | `-24.0%` | `STOP_LOSS_HIT` | $0.0676 |
| 16 | `LONG` | 2026-07-25 06:55:59 UTC | 2026-07-25 06:59:47 UTC | 3m 47s | `1.559` | `1.561` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0680 |
| 17 | `SHORT` | 2026-07-25 07:10:59 UTC | 2026-07-25 07:11:15 UTC | 15.2s | `1.558` | `1.556` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 18 | `LONG` | 2026-07-25 08:16:59 UTC | 2026-07-25 08:19:08 UTC | 2m 08s | `1.549` | `1.551` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.7%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 19 | `SHORT` | 2026-07-25 08:25:59 UTC | 2026-07-25 08:27:01 UTC | 1m 01s | `1.547` | `1.545` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.7%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 20 | `LONG` | 2026-07-25 09:01:59 UTC | 2026-07-25 09:10:08 UTC | 8m 08s | `1.543` | `1.545` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.7%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 21 | `SHORT` | 2026-07-25 10:07:59 UTC | 2026-07-25 10:10:15 UTC | 2m 15s | `1.546` | `1.551` | $0.31 | $0.00 | $0.000000 | **-0.0010** | `-24.3%` | `STOP_LOSS_HIT` | $0.0686 |
| 22 | `LONG` | 2026-07-25 10:20:59 UTC | 2026-07-25 10:25:32 UTC | 4m 32s | `1.550` | `1.552` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.7%` | `MIN_PROFIT_TP_HIT` | $0.0690 |
| 23 | `SHORT` | 2026-07-25 10:53:59 UTC | 2026-07-25 11:00:10 UTC | 6m 10s | `1.555` | `1.553` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0694 |
| 24 | `SHORT` | 2026-07-25 11:01:59 UTC | 2026-07-25 11:11:27 UTC | 9m 27s | `1.551` | `1.549` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.7%` | `MIN_PROFIT_TP_HIT` | $0.0698 |
| 25 | `LONG` | 2026-07-25 11:32:59 UTC | 2026-07-25 11:33:03 UTC | 3.5s | `1.550` | `1.552` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.7%` | `MIN_PROFIT_TP_HIT` | $0.0702 |
| ... | ... | *(1239 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 1265 | `SHORT` | 2026-08-14 17:53:59 UTC | 2026-08-14 17:55:43 UTC | 1m 43s | `1.426` | `1.424` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0958 |
| 1266 | `SHORT` | 2026-08-14 17:56:59 UTC | 2026-08-14 17:57:15 UTC | 15.5s | `1.421` | `1.419` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.6%` | `MIN_PROFIT_TP_HIT` | $0.0962 |
| 1267 | `LONG` | 2026-08-14 18:04:59 UTC | 2026-08-14 18:09:12 UTC | 4m 12s | `1.428` | `1.423` | $0.29 | $0.00 | $0.000000 | **-0.0010** | `-26.3%` | `STOP_LOSS_HIT` | $0.0952 |
| 1268 | `SHORT` | 2026-08-14 18:10:59 UTC | 2026-08-14 18:13:22 UTC | 2m 22s | `1.421` | `1.419` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.6%` | `MIN_PROFIT_TP_HIT` | $0.0956 |
| 1269 | `LONG` | 2026-08-14 18:18:59 UTC | 2026-08-14 18:23:00 UTC | 4m 00s | `1.427` | `1.429` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0960 |
| 1270 | `SHORT` | 2026-08-14 18:31:59 UTC | 2026-08-14 18:32:09 UTC | 9.5s | `1.422` | `1.420` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0964 |
| 1271 | `LONG` | 2026-08-14 18:41:59 UTC | 2026-08-14 18:47:54 UTC | 5m 54s | `1.426` | `1.421` | $0.29 | $0.00 | $0.000000 | **-0.0010** | `-26.3%` | `STOP_LOSS_HIT` | $0.0954 |
| 1272 | `SHORT` | 2026-08-14 18:48:59 UTC | 2026-08-14 18:52:46 UTC | 3m 46s | `1.420` | `1.425` | $0.28 | $0.00 | $0.000000 | **-0.0010** | `-26.4%` | `STOP_LOSS_HIT` | $0.0944 |
| 1273 | `LONG` | 2026-08-14 18:54:59 UTC | 2026-08-14 18:57:00 UTC | 2m 00s | `1.427` | `1.429` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0948 |
| 1274 | `SHORT` | 2026-08-14 19:04:59 UTC | 2026-08-14 19:19:30 UTC | 14m 30s | `1.424` | `1.422` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0952 |
| 1275 | `SHORT` | 2026-08-14 19:20:59 UTC | 2026-08-14 19:24:54 UTC | 3m 54s | `1.425` | `1.423` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0956 |
| 1276 | `SHORT` | 2026-08-14 19:25:59 UTC | 2026-08-14 19:27:03 UTC | 1m 03s | `1.425` | `1.423` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0960 |
| 1277 | `LONG` | 2026-08-14 19:37:59 UTC | 2026-08-14 19:57:03 UTC | 19m 03s | `1.426` | `1.428` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0964 |
| 1278 | `SHORT` | 2026-08-14 20:47:59 UTC | 2026-08-14 20:48:49 UTC | 49.1s | `1.446` | `1.451` | $0.29 | $0.00 | $0.000000 | **-0.0010** | `-25.9%` | `STOP_LOSS_HIT` | $0.0954 |
| 1279 | `LONG` | 2026-08-14 20:50:59 UTC | 2026-08-14 20:53:26 UTC | 2m 26s | `1.454` | `1.449` | $0.29 | $0.00 | $0.000000 | **-0.0010** | `-25.8%` | `STOP_LOSS_HIT` | $0.0944 |
| 1280 | `SHORT` | 2026-08-14 20:55:59 UTC | 2026-08-14 20:57:23 UTC | 1m 23s | `1.449` | `1.447` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.4%` | `MIN_PROFIT_TP_HIT` | $0.0948 |
| 1281 | `LONG` | 2026-08-14 21:02:59 UTC | 2026-08-14 21:03:19 UTC | 19.4s | `1.451` | `1.446` | $0.29 | $0.00 | $0.000000 | **-0.0010** | `-25.8%` | `STOP_LOSS_HIT` | $0.0938 |
| 1282 | `SHORT` | 2026-08-14 21:04:59 UTC | 2026-08-14 21:08:35 UTC | 3m 35s | `1.447` | `1.445` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.4%` | `MIN_PROFIT_TP_HIT` | $0.0942 |
| 1283 | `LONG` | 2026-08-14 21:52:59 UTC | 2026-08-14 21:58:25 UTC | 5m 25s | `1.430` | `1.432` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0946 |
| 1284 | `LONG` | 2026-08-14 22:01:59 UTC | 2026-08-14 22:06:40 UTC | 4m 40s | `1.433` | `1.428` | $0.29 | $0.00 | $0.000000 | **-0.0010** | `-26.2%` | `STOP_LOSS_HIT` | $0.0936 |
| 1285 | `SHORT` | 2026-08-14 22:07:59 UTC | 2026-08-14 22:13:43 UTC | 5m 43s | `1.428` | `1.426` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0940 |
| 1286 | `SHORT` | 2026-08-14 22:14:59 UTC | 2026-08-14 22:15:50 UTC | 50.9s | `1.425` | `1.423` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0944 |
| 1287 | `LONG` | 2026-08-14 22:37:59 UTC | 2026-08-14 23:01:43 UTC | 23m 43s | `1.423` | `1.425` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0948 |
| 1288 | `SHORT` | 2026-08-14 23:36:59 UTC | 2026-08-14 23:41:14 UTC | 4m 14s | `1.428` | `1.433` | $0.29 | $0.00 | $0.000000 | **-0.0010** | `-26.3%` | `STOP_LOSS_HIT` | $0.0938 |
| 1289 | `SHORT` | 2026-08-14 23:55:59 UTC | 2026-08-15 00:05:21 UTC | 9m 21s | `1.431` | `1.436` | $0.29 | $0.00 | $0.000000 | **-0.0010** | `-26.2%` | `STOP_LOSS_HIT` | $0.0928 |

> 💡 *Full granular dataset with all 1289 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
