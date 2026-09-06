# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:11:57 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.1212 USDT` | `₹11.45` | `+73.14%` |
| **Net Realized PnL** | **`+0.0512 USDT`** | **`₹+4.84`** | **`+73.14% Net ROI`** |
| **Gross Profit** | `+0.8912 USDT` | `₹84.17` | Total positive trade returns |
| **Gross Loss** | `-0.8400 USDT` | `₹79.34` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.06`** | — | Profitable |
| **Win / Loss Payoff** | `0.50` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0736 USDT` | `₹6.95` | **`-48.29%` Peak-to-Trough** |
| **Win Rate** | **`67.97%`** | — | `1114 Wins / 525 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `2.63` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `1.85` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `1.51` | — | Net ROI divided by Max Drawdown |

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
| **Take Profit Target** | `+4 ticks` (`+0.004 USDT`) | Guaranteed Min-Profit TP (`entry + N*pu`) |
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
| **Total Trades Executed** | `1639` | Total completed trade lifecycle events |
| **Winning Trades** | `1114` | `67.97%` of total trades |
| **Losing Trades** | `525` | `32.03%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0008 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0016 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0008 USDT (+18.1% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0016 USDT (-36.2% ROE)` | Trade #5 (SHORT) |
| **Max Consecutive Wins** | `20` trades | Peak winning streak |
| **Max Consecutive Losses** | `8` trades | Peak losing streak |
| **Average Trade Duration** | `14m 51s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `1.4s` | Trade #1219 |
| **Longest Trade In-Position** | `3h 41m 35s` | Trade #846 |
| **Cumulative Time In Position** | `405h 53m 23s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `826` (50.4%) | `813` (49.6%) | `1639` |
| **Wins / Losses** | `556 W / 270 L` | `558 W / 255 L` | `1114 W / 525 L` |
| **Win Rate** | **`67.31%`** | **`68.63%`** | **`67.97%`** |
| **Gross Profit** | `+0.4448 USDT` | `+0.4464 USDT` | `+0.8912 USDT` |
| **Gross Loss** | `-0.4320 USDT` | `-0.4080 USDT` | `-0.8400 USDT` |
| **Net Realized PnL** | **`+0.0128 USDT`** | **`+0.0384 USDT`** | **`+0.0512 USDT`** |
| **Net PnL (INR)** | `₹+1.21` | `₹+3.63` | `₹+4.84` |
| **Profit Factor** | `1.03` | `1.09` | `1.06` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1114` | `68.0%` | `+0.8912 USDT` | `₹+84.17` | `100.0%` | `12m 36s` |
| `STOP_LOSS_HIT` | `525` | `32.0%` | `-0.8400 USDT` | `₹-79.34` | `0.0%` | `19m 38s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:30:53 UTC | 1m 53s | `1.661` | `1.665` | $0.33 | $0.00 | $0.000000 | **+0.0008** | `+18.1%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 01:09:27 UTC | 32m 27s | `1.664` | `1.660` | $0.33 | $0.00 | $0.000000 | **+0.0008** | `+18.0%` | `MIN_PROFIT_TP_HIT` | $0.0716 |
| 3 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:07 UTC | 7.5s | `1.645` | `1.649` | $0.33 | $0.00 | $0.000000 | **+0.0008** | `+18.2%` | `MIN_PROFIT_TP_HIT` | $0.0724 |
| 4 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:24:48 UTC | 1m 48s | `1.658` | `1.654` | $0.33 | $0.00 | $0.000000 | **+0.0008** | `+18.1%` | `MIN_PROFIT_TP_HIT` | $0.0732 |
| 5 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:38:45 UTC | 3m 45s | `1.658` | `1.666` | $0.33 | $0.00 | $0.000000 | **-0.0016** | `-36.2%` | `STOP_LOSS_HIT` | $0.0716 |
| 6 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 02:02:52 UTC | 14m 52s | `1.676` | `1.684` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.8%` | `STOP_LOSS_HIT` | $0.0700 |
| 7 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:10:33 UTC | 6m 33s | `1.685` | `1.689` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.8%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 8 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:31:24 UTC | 13m 24s | `1.702` | `1.710` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.3%` | `STOP_LOSS_HIT` | $0.0692 |
| 9 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:46 UTC | 46.0s | `1.704` | `1.708` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.6%` | `MIN_PROFIT_TP_HIT` | $0.0700 |
| 10 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:18 UTC | 3m 18s | `1.697` | `1.701` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.7%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 11 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:39 UTC | 39.6s | `1.704` | `1.712` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.2%` | `STOP_LOSS_HIT` | $0.0692 |
| 12 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:32 UTC | 32.4s | `1.707` | `1.715` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.1%` | `STOP_LOSS_HIT` | $0.0676 |
| 13 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:11 UTC | 11.4s | `1.729` | `1.725` | $0.35 | $0.00 | $0.000000 | **+0.0008** | `+17.4%` | `MIN_PROFIT_TP_HIT` | $0.0684 |
| 14 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:30 UTC | 30.3s | `1.711` | `1.703` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.1%` | `STOP_LOSS_HIT` | $0.0668 |
| 15 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:24:02 UTC | 4m 02s | `1.704` | `1.696` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.2%` | `STOP_LOSS_HIT` | $0.0652 |
| 16 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:36:36 UTC | 8m 36s | `1.699` | `1.703` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.7%` | `MIN_PROFIT_TP_HIT` | $0.0660 |
| 17 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:52:16 UTC | 10m 16s | `1.706` | `1.714` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.2%` | `STOP_LOSS_HIT` | $0.0644 |
| 18 | `SHORT` | 2026-07-01 03:56:59 UTC | 2026-07-01 03:57:15 UTC | 15.0s | `1.712` | `1.708` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.5%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 19 | `LONG` | 2026-07-01 04:02:59 UTC | 2026-07-01 04:10:10 UTC | 7m 10s | `1.705` | `1.697` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.2%` | `STOP_LOSS_HIT` | $0.0636 |
| 20 | `LONG` | 2026-07-01 04:11:59 UTC | 2026-07-01 04:17:10 UTC | 5m 10s | `1.700` | `1.704` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.6%` | `MIN_PROFIT_TP_HIT` | $0.0644 |
| 21 | `SHORT` | 2026-07-01 04:21:59 UTC | 2026-07-01 04:37:14 UTC | 15m 14s | `1.704` | `1.700` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.6%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 22 | `LONG` | 2026-07-01 04:38:59 UTC | 2026-07-01 04:59:36 UTC | 20m 36s | `1.700` | `1.704` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.6%` | `MIN_PROFIT_TP_HIT` | $0.0660 |
| 23 | `LONG` | 2026-07-01 05:06:59 UTC | 2026-07-01 05:26:59 UTC | 19m 59s | `1.705` | `1.697` | $0.34 | $0.00 | $0.000000 | **-0.0016** | `-35.2%` | `STOP_LOSS_HIT` | $0.0644 |
| 24 | `LONG` | 2026-07-01 05:28:59 UTC | 2026-07-01 05:48:36 UTC | 19m 36s | `1.706` | `1.710` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.6%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 25 | `SHORT` | 2026-07-01 05:52:59 UTC | 2026-07-01 06:02:34 UTC | 9m 34s | `1.712` | `1.708` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.5%` | `MIN_PROFIT_TP_HIT` | $0.0660 |
| ... | ... | *(1589 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 1615 | `LONG` | 2026-07-23 16:58:59 UTC | 2026-07-23 17:02:07 UTC | 3m 07s | `1.631` | `1.623` | $0.33 | $0.00 | $0.000000 | **-0.0016** | `-36.8%` | `STOP_LOSS_HIT` | $0.1188 |
| 1616 | `LONG` | 2026-07-23 17:04:59 UTC | 2026-07-23 17:40:40 UTC | 35m 40s | `1.621` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.0%` | `STOP_LOSS_HIT` | $0.1172 |
| 1617 | `SHORT` | 2026-07-23 17:47:59 UTC | 2026-07-23 17:55:25 UTC | 7m 25s | `1.611` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.1180 |
| 1618 | `LONG` | 2026-07-23 18:02:59 UTC | 2026-07-23 18:05:47 UTC | 2m 47s | `1.599` | `1.591` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.5%` | `STOP_LOSS_HIT` | $0.1164 |
| 1619 | `SHORT` | 2026-07-23 18:12:59 UTC | 2026-07-23 18:17:33 UTC | 4m 33s | `1.594` | `1.590` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.8%` | `MIN_PROFIT_TP_HIT` | $0.1172 |
| 1620 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:41:11 UTC | 12m 11s | `1.610` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.1180 |
| 1621 | `LONG` | 2026-07-23 18:46:59 UTC | 2026-07-23 18:49:06 UTC | 2m 06s | `1.606` | `1.610` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1188 |
| 1622 | `SHORT` | 2026-07-23 18:51:59 UTC | 2026-07-23 19:25:52 UTC | 33m 52s | `1.608` | `1.616` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.3%` | `STOP_LOSS_HIT` | $0.1172 |
| 1623 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:41:22 UTC | 12m 22s | `1.616` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.1180 |
| 1624 | `LONG` | 2026-07-23 19:45:59 UTC | 2026-07-23 19:59:06 UTC | 13m 06s | `1.612` | `1.616` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.1188 |
| 1625 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:40:29 UTC | 29m 29s | `1.623` | `1.619` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.5%` | `MIN_PROFIT_TP_HIT` | $0.1196 |
| 1626 | `LONG` | 2026-07-23 20:45:59 UTC | 2026-07-23 20:54:24 UTC | 8m 24s | `1.618` | `1.622` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.5%` | `MIN_PROFIT_TP_HIT` | $0.1204 |
| 1627 | `SHORT` | 2026-07-23 20:57:59 UTC | 2026-07-23 21:08:20 UTC | 10m 20s | `1.623` | `1.619` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.5%` | `MIN_PROFIT_TP_HIT` | $0.1212 |
| 1628 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:31:59 UTC | 13m 59s | `1.617` | `1.609` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.1%` | `STOP_LOSS_HIT` | $0.1196 |
| 1629 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:46:15 UTC | 8m 15s | `1.603` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1204 |
| 1630 | `SHORT` | 2026-07-23 21:48:59 UTC | 2026-07-23 22:06:10 UTC | 17m 10s | `1.605` | `1.613` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.4%` | `STOP_LOSS_HIT` | $0.1188 |
| 1631 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:55 UTC | 5m 55s | `1.611` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.1196 |
| 1632 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:20:50 UTC | 1m 50s | `1.607` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1204 |
| 1633 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:30:35 UTC | 2m 35s | `1.616` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.1212 |
| 1634 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:38:25 UTC | 3m 25s | `1.611` | `1.603` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.2%` | `STOP_LOSS_HIT` | $0.1196 |
| 1635 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:44:34 UTC | 3m 34s | `1.604` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1204 |
| 1636 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:04:35 UTC | 14m 35s | `1.607` | `1.603` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1212 |
| 1637 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:25:35 UTC | 16m 35s | `1.605` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1220 |
| 1638 | `SHORT` | 2026-07-23 23:29:59 UTC | 2026-07-23 23:47:35 UTC | 17m 35s | `1.608` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.1228 |
| 1639 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:06:03 UTC | 11m 03s | `1.599` | `1.591` | $0.32 | $0.00 | $0.000000 | **-0.0016** | `-37.5%` | `STOP_LOSS_HIT` | $0.1212 |

> 💡 *Full granular dataset with all 1639 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
