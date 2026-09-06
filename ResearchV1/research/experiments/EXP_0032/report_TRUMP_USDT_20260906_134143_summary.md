# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:11:43 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.0556 USDT` | `₹5.25` | `-20.57%` |
| **Net Realized PnL** | **`-0.0144 USDT`** | **`₹-1.36`** | **`-20.57% Net ROI`** |
| **Gross Profit** | `+0.9480 USDT` | `₹89.54` | Total positive trade returns |
| **Gross Loss** | `-0.9624 USDT` | `₹90.90` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`0.99`** | — | Unprofitable / Needs Optimization |
| **Win / Loss Payoff** | `0.67` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0900 USDT` | `₹8.50` | **`-82.42%` Peak-to-Trough** |
| **Win Rate** | **`59.64%`** | — | `1185 Wins / 802 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `0.35` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `0.29` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `-0.25` | — | Net ROI divided by Max Drawdown |

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
| **Total Trades Executed** | `1987` | Total completed trade lifecycle events |
| **Winning Trades** | `1185` | `59.64%` of total trades |
| **Losing Trades** | `802` | `40.36%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `-0.0000 USDT` (`₹-0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0008 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0012 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0008 USDT (+18.1% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0012 USDT (-27.0% ROE)` | Trade #2 (SHORT) |
| **Max Consecutive Wins** | `12` trades | Peak winning streak |
| **Max Consecutive Losses** | `8` trades | Peak losing streak |
| **Average Trade Duration** | `11m 14s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `1.4s` | Trade #1494 |
| **Longest Trade In-Position** | `2h 47m 59s` | Trade #1447 |
| **Cumulative Time In Position** | `372h 11m 35s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `982` (49.4%) | `1005` (50.6%) | `1987` |
| **Wins / Losses** | `581 W / 401 L` | `604 W / 401 L` | `1185 W / 802 L` |
| **Win Rate** | **`59.16%`** | **`60.10%`** | **`59.64%`** |
| **Gross Profit** | `+0.4648 USDT` | `+0.4832 USDT` | `+0.9480 USDT` |
| **Gross Loss** | `-0.4812 USDT` | `-0.4812 USDT` | `-0.9624 USDT` |
| **Net Realized PnL** | **`-0.0164 USDT`** | **`+0.0020 USDT`** | **`-0.0144 USDT`** |
| **Net PnL (INR)** | `₹-1.55` | `₹+0.19` | `₹-1.36` |
| **Profit Factor** | `0.97` | `1.00` | `0.99` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1185` | `59.6%` | `+0.9480 USDT` | `₹+89.54` | `100.0%` | `9m 44s` |
| `STOP_LOSS_HIT` | `802` | `40.4%` | `-0.9624 USDT` | `₹-90.90` | `0.0%` | `13m 27s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:30:53 UTC | 1m 53s | `1.661` | `1.665` | $0.33 | $0.00 | $0.000000 | **+0.0008** | `+18.1%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 2 | `SHORT` | 2026-07-01 00:36:59 UTC | 2026-07-01 00:52:46 UTC | 15m 46s | `1.664` | `1.670` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.0%` | `STOP_LOSS_HIT` | $0.0696 |
| 3 | `SHORT` | 2026-07-01 00:55:59 UTC | 2026-07-01 00:58:49 UTC | 2m 49s | `1.669` | `1.665` | $0.33 | $0.00 | $0.000000 | **+0.0008** | `+18.0%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 4 | `LONG` | 2026-07-01 01:01:59 UTC | 2026-07-01 01:07:03 UTC | 5m 03s | `1.667` | `1.661` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.0%` | `STOP_LOSS_HIT` | $0.0692 |
| 5 | `LONG` | 2026-07-01 01:09:59 UTC | 2026-07-01 01:12:29 UTC | 2m 29s | `1.661` | `1.655` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.1%` | `STOP_LOSS_HIT` | $0.0680 |
| 6 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:07 UTC | 7.5s | `1.645` | `1.649` | $0.33 | $0.00 | $0.000000 | **+0.0008** | `+18.2%` | `MIN_PROFIT_TP_HIT` | $0.0688 |
| 7 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:24:48 UTC | 1m 48s | `1.658` | `1.654` | $0.33 | $0.00 | $0.000000 | **+0.0008** | `+18.1%` | `MIN_PROFIT_TP_HIT` | $0.0696 |
| 8 | `SHORT` | 2026-07-01 01:34:59 UTC | 2026-07-01 01:37:07 UTC | 2m 07s | `1.658` | `1.664` | $0.33 | $0.00 | $0.000000 | **-0.0012** | `-27.1%` | `STOP_LOSS_HIT` | $0.0684 |
| 9 | `SHORT` | 2026-07-01 01:47:59 UTC | 2026-07-01 01:56:02 UTC | 8m 02s | `1.676` | `1.682` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.8%` | `STOP_LOSS_HIT` | $0.0672 |
| 10 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 02:02:52 UTC | 3m 52s | `1.678` | `1.684` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.8%` | `STOP_LOSS_HIT` | $0.0660 |
| 11 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:06:09 UTC | 2m 09s | `1.685` | `1.679` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.7%` | `STOP_LOSS_HIT` | $0.0648 |
| 12 | `LONG` | 2026-07-01 02:08:59 UTC | 2026-07-01 02:10:07 UTC | 1m 07s | `1.684` | `1.688` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.8%` | `MIN_PROFIT_TP_HIT` | $0.0656 |
| 13 | `SHORT` | 2026-07-01 02:17:59 UTC | 2026-07-01 02:22:05 UTC | 4m 05s | `1.702` | `1.708` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0644 |
| 14 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:31:16 UTC | 1m 16s | `1.705` | `1.709` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.6%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 15 | `LONG` | 2026-07-01 02:34:59 UTC | 2026-07-01 02:35:46 UTC | 46.0s | `1.704` | `1.708` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.6%` | `MIN_PROFIT_TP_HIT` | $0.0660 |
| 16 | `LONG` | 2026-07-01 02:40:59 UTC | 2026-07-01 02:44:18 UTC | 3m 18s | `1.697` | `1.701` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.7%` | `MIN_PROFIT_TP_HIT` | $0.0668 |
| 17 | `SHORT` | 2026-07-01 03:00:59 UTC | 2026-07-01 03:01:38 UTC | 38.4s | `1.704` | `1.710` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0656 |
| 18 | `SHORT` | 2026-07-01 03:04:59 UTC | 2026-07-01 03:05:24 UTC | 24.3s | `1.707` | `1.713` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0644 |
| 19 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:11 UTC | 11.4s | `1.729` | `1.725` | $0.35 | $0.00 | $0.000000 | **+0.0008** | `+17.4%` | `MIN_PROFIT_TP_HIT` | $0.0652 |
| 20 | `LONG` | 2026-07-01 03:15:59 UTC | 2026-07-01 03:16:27 UTC | 28.0s | `1.711` | `1.705` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.3%` | `STOP_LOSS_HIT` | $0.0640 |
| 21 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:23:46 UTC | 3m 46s | `1.704` | `1.698` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0628 |
| 22 | `LONG` | 2026-07-01 03:27:59 UTC | 2026-07-01 03:36:36 UTC | 8m 36s | `1.699` | `1.703` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.7%` | `MIN_PROFIT_TP_HIT` | $0.0636 |
| 23 | `SHORT` | 2026-07-01 03:41:59 UTC | 2026-07-01 03:47:31 UTC | 5m 31s | `1.706` | `1.712` | $0.34 | $0.00 | $0.000000 | **-0.0012** | `-26.4%` | `STOP_LOSS_HIT` | $0.0624 |
| 24 | `LONG` | 2026-07-01 03:51:59 UTC | 2026-07-01 03:52:23 UTC | 23.6s | `1.711` | `1.715` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.5%` | `MIN_PROFIT_TP_HIT` | $0.0632 |
| 25 | `SHORT` | 2026-07-01 03:56:59 UTC | 2026-07-01 03:57:15 UTC | 15.0s | `1.712` | `1.708` | $0.34 | $0.00 | $0.000000 | **+0.0008** | `+17.5%` | `MIN_PROFIT_TP_HIT` | $0.0640 |
| ... | ... | *(1937 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 1963 | `LONG` | 2026-07-23 17:04:59 UTC | 2026-07-23 17:37:19 UTC | 32m 19s | `1.621` | `1.615` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-27.8%` | `STOP_LOSS_HIT` | $0.0484 |
| 1964 | `SHORT` | 2026-07-23 17:47:59 UTC | 2026-07-23 17:55:25 UTC | 7m 25s | `1.611` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.0492 |
| 1965 | `LONG` | 2026-07-23 18:02:59 UTC | 2026-07-23 18:05:38 UTC | 2m 38s | `1.599` | `1.593` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-28.1%` | `STOP_LOSS_HIT` | $0.0480 |
| 1966 | `SHORT` | 2026-07-23 18:12:59 UTC | 2026-07-23 18:17:33 UTC | 4m 33s | `1.594` | `1.590` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.8%` | `MIN_PROFIT_TP_HIT` | $0.0488 |
| 1967 | `SHORT` | 2026-07-23 18:28:59 UTC | 2026-07-23 18:41:11 UTC | 12m 11s | `1.610` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.0496 |
| 1968 | `LONG` | 2026-07-23 18:46:59 UTC | 2026-07-23 18:49:06 UTC | 2m 06s | `1.606` | `1.610` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.0504 |
| 1969 | `SHORT` | 2026-07-23 18:51:59 UTC | 2026-07-23 19:25:50 UTC | 33m 50s | `1.608` | `1.614` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-28.0%` | `STOP_LOSS_HIT` | $0.0492 |
| 1970 | `SHORT` | 2026-07-23 19:28:59 UTC | 2026-07-23 19:41:22 UTC | 12m 22s | `1.616` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.0500 |
| 1971 | `LONG` | 2026-07-23 19:45:59 UTC | 2026-07-23 19:59:06 UTC | 13m 06s | `1.612` | `1.616` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.0508 |
| 1972 | `SHORT` | 2026-07-23 20:10:59 UTC | 2026-07-23 20:40:29 UTC | 29m 29s | `1.623` | `1.619` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.5%` | `MIN_PROFIT_TP_HIT` | $0.0516 |
| 1973 | `LONG` | 2026-07-23 20:45:59 UTC | 2026-07-23 20:54:24 UTC | 8m 24s | `1.618` | `1.622` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.5%` | `MIN_PROFIT_TP_HIT` | $0.0524 |
| 1974 | `SHORT` | 2026-07-23 20:57:59 UTC | 2026-07-23 21:08:20 UTC | 10m 20s | `1.623` | `1.619` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.5%` | `MIN_PROFIT_TP_HIT` | $0.0532 |
| 1975 | `LONG` | 2026-07-23 21:17:59 UTC | 2026-07-23 21:29:06 UTC | 11m 06s | `1.617` | `1.611` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-27.8%` | `STOP_LOSS_HIT` | $0.0520 |
| 1976 | `SHORT` | 2026-07-23 21:30:59 UTC | 2026-07-23 21:32:45 UTC | 1m 45s | `1.610` | `1.606` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.0528 |
| 1977 | `LONG` | 2026-07-23 21:37:59 UTC | 2026-07-23 21:46:15 UTC | 8m 15s | `1.603` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.0536 |
| 1978 | `SHORT` | 2026-07-23 21:48:59 UTC | 2026-07-23 22:05:02 UTC | 16m 02s | `1.605` | `1.611` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-28.0%` | `STOP_LOSS_HIT` | $0.0524 |
| 1979 | `SHORT` | 2026-07-23 22:11:59 UTC | 2026-07-23 22:17:55 UTC | 5m 55s | `1.611` | `1.607` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.0532 |
| 1980 | `LONG` | 2026-07-23 22:18:59 UTC | 2026-07-23 22:20:50 UTC | 1m 50s | `1.607` | `1.611` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.0540 |
| 1981 | `SHORT` | 2026-07-23 22:27:59 UTC | 2026-07-23 22:30:35 UTC | 2m 35s | `1.616` | `1.612` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.6%` | `MIN_PROFIT_TP_HIT` | $0.0548 |
| 1982 | `LONG` | 2026-07-23 22:34:59 UTC | 2026-07-23 22:37:43 UTC | 2m 43s | `1.611` | `1.605` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-27.9%` | `STOP_LOSS_HIT` | $0.0536 |
| 1983 | `LONG` | 2026-07-23 22:40:59 UTC | 2026-07-23 22:44:34 UTC | 3m 34s | `1.604` | `1.608` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.0544 |
| 1984 | `SHORT` | 2026-07-23 22:49:59 UTC | 2026-07-23 23:04:35 UTC | 14m 35s | `1.607` | `1.603` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.0552 |
| 1985 | `LONG` | 2026-07-23 23:08:59 UTC | 2026-07-23 23:25:35 UTC | 16m 35s | `1.605` | `1.609` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.0560 |
| 1986 | `SHORT` | 2026-07-23 23:29:59 UTC | 2026-07-23 23:47:35 UTC | 17m 35s | `1.608` | `1.604` | $0.32 | $0.00 | $0.000000 | **+0.0008** | `+18.7%` | `MIN_PROFIT_TP_HIT` | $0.0568 |
| 1987 | `LONG` | 2026-07-23 23:54:59 UTC | 2026-07-24 00:05:54 UTC | 10m 54s | `1.599` | `1.593` | $0.32 | $0.00 | $0.000000 | **-0.0012** | `-28.1%` | `STOP_LOSS_HIT` | $0.0556 |

> 💡 *Full granular dataset with all 1987 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
