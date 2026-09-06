# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:17:50 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.1088 USDT` | `₹10.28` | `+55.43%` |
| **Net Realized PnL** | **`+0.0388 USDT`** | **`₹+3.66`** | **`+55.43% Net ROI`** |
| **Gross Profit** | `+0.5780 USDT` | `₹54.59` | Total positive trade returns |
| **Gross Loss** | `-0.5392 USDT` | `₹50.93` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.07`** | — | Profitable |
| **Win / Loss Payoff** | `1.00` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0140 USDT` | `₹1.32` | **`-19.66%` Peak-to-Trough** |
| **Win Rate** | **`51.74%`** | — | `1445 Wins / 1348 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `2.77` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `2.77` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `2.82` | — | Net ROI divided by Max Drawdown |

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
| **Stop Loss Rule** | `-2 ticks away from entry (0.002 USDT)` | Stop loss evaluation logic |

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
| **Total Trades Executed** | `2793` | Total completed trade lifecycle events |
| **Winning Trades** | `1445` | `51.74%` of total trades |
| **Losing Trades** | `1348` | `48.26%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0004 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+7.1% ROE)` | Trade #999 (SHORT) |
| **Largest Losing Trade** | `-0.0004 USDT (-6.8% ROE)` | Trade #1004 (LONG) |
| **Max Consecutive Wins** | `11` trades | Peak winning streak |
| **Max Consecutive Losses** | `9` trades | Peak losing streak |
| **Average Trade Duration** | `50.0s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #558 |
| **Longest Trade In-Position** | `36m 10s` | Trade #489 |
| **Cumulative Time In Position** | `38h 49m 32s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1418` (50.8%) | `1375` (49.2%) | `2793` |
| **Wins / Losses** | `733 W / 685 L` | `712 W / 663 L` | `1445 W / 1348 L` |
| **Win Rate** | **`51.69%`** | **`51.78%`** | **`51.74%`** |
| **Gross Profit** | `+0.2932 USDT` | `+0.2848 USDT` | `+0.5780 USDT` |
| **Gross Loss** | `-0.2740 USDT` | `-0.2652 USDT` | `-0.5392 USDT` |
| **Net Realized PnL** | **`+0.0192 USDT`** | **`+0.0196 USDT`** | **`+0.0388 USDT`** |
| **Net PnL (INR)** | `₹+1.81` | `₹+1.85` | `₹+3.66` |
| **Profit Factor** | `1.07` | `1.07` | `1.07` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1445` | `51.7%` | `+0.5780 USDT` | `₹+54.59` | `100.0%` | `51.4s` |
| `STOP_LOSS_HIT` | `1348` | `48.3%` | `-0.5392 USDT` | `₹-50.93` | `0.0%` | `48.6s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-08-16 00:26:59 UTC | 2026-08-16 00:27:20 UTC | 20.3s | `1.409` | `1.411` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.6%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-08-16 00:31:59 UTC | 2026-08-16 00:40:07 UTC | 8m 07s | `1.410` | `1.408` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.6%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 3 | `LONG` | 2026-08-16 00:44:59 UTC | 2026-08-16 00:49:32 UTC | 4m 32s | `1.408` | `1.406` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.7%` | `STOP_LOSS_HIT` | $0.0704 |
| 4 | `SHORT` | 2026-08-16 00:56:59 UTC | 2026-08-16 01:01:28 UTC | 4m 28s | `1.410` | `1.412` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.6%` | `STOP_LOSS_HIT` | $0.0700 |
| 5 | `LONG` | 2026-08-16 01:17:59 UTC | 2026-08-16 01:18:48 UTC | 48.9s | `1.403` | `1.405` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 6 | `SHORT` | 2026-08-16 01:22:59 UTC | 2026-08-16 01:26:18 UTC | 3m 18s | `1.402` | `1.400` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 7 | `LONG` | 2026-08-16 01:32:59 UTC | 2026-08-16 01:33:06 UTC | 6.9s | `1.393` | `1.395` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 8 | `SHORT` | 2026-08-16 01:38:59 UTC | 2026-08-16 01:40:50 UTC | 1m 50s | `1.392` | `1.394` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.8%` | `STOP_LOSS_HIT` | $0.0708 |
| 9 | `SHORT` | 2026-08-16 01:47:59 UTC | 2026-08-16 01:51:25 UTC | 3m 25s | `1.395` | `1.397` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.8%` | `STOP_LOSS_HIT` | $0.0704 |
| 10 | `LONG` | 2026-08-16 01:59:59 UTC | 2026-08-16 02:02:38 UTC | 2m 38s | `1.395` | `1.393` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.8%` | `STOP_LOSS_HIT` | $0.0700 |
| 11 | `LONG` | 2026-08-16 02:05:59 UTC | 2026-08-16 02:10:03 UTC | 4m 03s | `1.392` | `1.394` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 12 | `LONG` | 2026-08-16 02:16:59 UTC | 2026-08-16 02:20:11 UTC | 3m 11s | `1.390` | `1.392` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 13 | `SHORT` | 2026-08-16 02:29:59 UTC | 2026-08-16 02:45:38 UTC | 15m 38s | `1.395` | `1.393` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 14 | `LONG` | 2026-08-16 02:48:59 UTC | 2026-08-16 03:01:52 UTC | 12m 52s | `1.393` | `1.391` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.8%` | `STOP_LOSS_HIT` | $0.0708 |
| 15 | `SHORT` | 2026-08-16 03:08:59 UTC | 2026-08-16 03:11:46 UTC | 2m 46s | `1.394` | `1.396` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.8%` | `STOP_LOSS_HIT` | $0.0704 |
| 16 | `LONG` | 2026-08-16 03:17:59 UTC | 2026-08-16 03:25:42 UTC | 7m 42s | `1.393` | `1.391` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.8%` | `STOP_LOSS_HIT` | $0.0700 |
| 17 | `SHORT` | 2026-08-16 03:36:59 UTC | 2026-08-16 03:39:09 UTC | 2m 09s | `1.395` | `1.397` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.8%` | `STOP_LOSS_HIT` | $0.0696 |
| 18 | `LONG` | 2026-08-16 03:40:59 UTC | 2026-08-16 03:52:02 UTC | 11m 02s | `1.395` | `1.393` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.8%` | `STOP_LOSS_HIT` | $0.0692 |
| 19 | `LONG` | 2026-08-16 03:56:59 UTC | 2026-08-16 04:00:05 UTC | 3m 05s | `1.394` | `1.392` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.8%` | `STOP_LOSS_HIT` | $0.0688 |
| 20 | `SHORT` | 2026-08-16 04:07:59 UTC | 2026-08-16 04:17:06 UTC | 9m 06s | `1.391` | `1.389` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.8%` | `MIN_PROFIT_TP_HIT` | $0.0692 |
| 21 | `SHORT` | 2026-08-16 04:23:59 UTC | 2026-08-16 04:25:54 UTC | 1m 54s | `1.392` | `1.394` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.8%` | `STOP_LOSS_HIT` | $0.0688 |
| 22 | `SHORT` | 2026-08-16 04:32:59 UTC | 2026-08-16 04:38:06 UTC | 5m 06s | `1.394` | `1.396` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.8%` | `STOP_LOSS_HIT` | $0.0684 |
| 23 | `SHORT` | 2026-08-16 04:42:59 UTC | 2026-08-16 04:43:10 UTC | 10.0s | `1.399` | `1.401` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.7%` | `STOP_LOSS_HIT` | $0.0680 |
| 24 | `LONG` | 2026-08-16 04:50:59 UTC | 2026-08-16 04:54:13 UTC | 3m 13s | `1.400` | `1.398` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.7%` | `STOP_LOSS_HIT` | $0.0676 |
| 25 | `LONG` | 2026-08-16 05:00:59 UTC | 2026-08-16 05:02:20 UTC | 1m 20s | `1.397` | `1.399` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.7%` | `MIN_PROFIT_TP_HIT` | $0.0680 |
| ... | ... | *(2743 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2769 | `SHORT` | 2026-08-30 20:40:59 UTC | 2026-08-30 20:41:14 UTC | 14.5s | `2.514` | `2.516` | $0.50 | $0.01 | $0.000000 | **-0.0004** | `-6.0%` | `STOP_LOSS_HIT` | $0.1088 |
| 2770 | `LONG` | 2026-08-30 20:46:59 UTC | 2026-08-30 20:47:01 UTC | 1.6s | `2.518` | `2.516` | $0.50 | $0.01 | $0.000000 | **-0.0004** | `-6.0%` | `STOP_LOSS_HIT` | $0.1084 |
| 2771 | `SHORT` | 2026-08-30 20:50:59 UTC | 2026-08-30 20:51:06 UTC | 6.9s | `2.525` | `2.527` | $0.51 | $0.01 | $0.000000 | **-0.0004** | `-5.9%` | `STOP_LOSS_HIT` | $0.1080 |
| 2772 | `SHORT` | 2026-08-30 20:54:59 UTC | 2026-08-30 20:56:09 UTC | 1m 09s | `2.525` | `2.527` | $0.51 | $0.01 | $0.000000 | **-0.0004** | `-5.9%` | `STOP_LOSS_HIT` | $0.1076 |
| 2773 | `LONG` | 2026-08-30 21:03:59 UTC | 2026-08-30 21:04:03 UTC | 3.9s | `2.500` | `2.502` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1080 |
| 2774 | `SHORT` | 2026-08-30 21:15:59 UTC | 2026-08-30 21:16:07 UTC | 7.4s | `2.503` | `2.501` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1084 |
| 2775 | `SHORT` | 2026-08-30 21:32:59 UTC | 2026-08-30 21:33:09 UTC | 9.9s | `2.509` | `2.507` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1088 |
| 2776 | `SHORT` | 2026-08-30 21:35:59 UTC | 2026-08-30 21:36:51 UTC | 51.1s | `2.510` | `2.512` | $0.50 | $0.01 | $0.000000 | **-0.0004** | `-6.0%` | `STOP_LOSS_HIT` | $0.1084 |
| 2777 | `LONG` | 2026-08-30 21:50:59 UTC | 2026-08-30 21:51:00 UTC | 0.5s | `2.488` | `2.490` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1088 |
| 2778 | `SHORT` | 2026-08-30 21:58:59 UTC | 2026-08-30 21:59:02 UTC | 2.5s | `2.506` | `2.508` | $0.50 | $0.01 | $0.000000 | **-0.0004** | `-6.0%` | `STOP_LOSS_HIT` | $0.1084 |
| 2779 | `LONG` | 2026-08-30 22:09:59 UTC | 2026-08-30 22:10:03 UTC | 3.7s | `2.516` | `2.518` | $0.50 | $0.01 | $0.000000 | **+0.0004** | `+6.0%` | `MIN_PROFIT_TP_HIT` | $0.1088 |
| 2780 | `LONG` | 2026-08-30 22:19:59 UTC | 2026-08-30 22:20:18 UTC | 18.2s | `2.501` | `2.499` | $0.50 | $0.01 | $0.000000 | **-0.0004** | `-6.0%` | `STOP_LOSS_HIT` | $0.1084 |
| 2781 | `SHORT` | 2026-08-30 22:43:59 UTC | 2026-08-30 22:44:04 UTC | 4.8s | `2.429` | `2.427` | $0.49 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1088 |
| 2782 | `LONG` | 2026-08-30 22:51:59 UTC | 2026-08-30 22:52:04 UTC | 4.7s | `2.416` | `2.418` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1092 |
| 2783 | `SHORT` | 2026-08-30 22:56:59 UTC | 2026-08-30 22:57:22 UTC | 22.4s | `2.424` | `2.426` | $0.48 | $0.01 | $0.000000 | **-0.0004** | `-6.2%` | `STOP_LOSS_HIT` | $0.1088 |
| 2784 | `SHORT` | 2026-08-30 23:00:59 UTC | 2026-08-30 23:01:00 UTC | 0.4s | `2.409` | `2.411` | $0.48 | $0.01 | $0.000000 | **-0.0004** | `-6.2%` | `STOP_LOSS_HIT` | $0.1084 |
| 2785 | `SHORT` | 2026-08-30 23:10:59 UTC | 2026-08-30 23:11:01 UTC | 1.1s | `2.405` | `2.407` | $0.48 | $0.01 | $0.000000 | **-0.0004** | `-6.2%` | `STOP_LOSS_HIT` | $0.1080 |
| 2786 | `SHORT` | 2026-08-30 23:15:59 UTC | 2026-08-30 23:16:00 UTC | 0.8s | `2.422` | `2.420` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1084 |
| 2787 | `SHORT` | 2026-08-30 23:18:59 UTC | 2026-08-30 23:19:00 UTC | 0.6s | `2.415` | `2.413` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.2%` | `MIN_PROFIT_TP_HIT` | $0.1088 |
| 2788 | `SHORT` | 2026-08-30 23:24:59 UTC | 2026-08-30 23:25:00 UTC | 0.4s | `2.414` | `2.416` | $0.48 | $0.01 | $0.000000 | **-0.0004** | `-6.2%` | `STOP_LOSS_HIT` | $0.1084 |
| 2789 | `LONG` | 2026-08-30 23:32:59 UTC | 2026-08-30 23:33:01 UTC | 1.6s | `2.388` | `2.390` | $0.48 | $0.01 | $0.000000 | **+0.0004** | `+6.3%` | `MIN_PROFIT_TP_HIT` | $0.1088 |
| 2790 | `LONG` | 2026-08-30 23:42:59 UTC | 2026-08-30 23:43:00 UTC | 0.7s | `2.330` | `2.328` | $0.47 | $0.01 | $0.000000 | **-0.0004** | `-6.4%` | `STOP_LOSS_HIT` | $0.1084 |
| 2791 | `SHORT` | 2026-08-30 23:53:59 UTC | 2026-08-30 23:54:11 UTC | 11.8s | `2.330` | `2.328` | $0.47 | $0.01 | $0.000000 | **+0.0004** | `+6.4%` | `MIN_PROFIT_TP_HIT` | $0.1088 |
| 2792 | `SHORT` | 2026-08-30 23:57:59 UTC | 2026-08-30 23:58:00 UTC | 0.5s | `2.343` | `2.341` | $0.47 | $0.01 | $0.000000 | **+0.0004** | `+6.4%` | `MIN_PROFIT_TP_HIT` | $0.1092 |
| 2793 | `SHORT` | 2026-08-31 00:00:59 UTC | 2026-08-31 00:01:00 UTC | 0.9s | `2.338` | `2.340` | $0.47 | $0.01 | $0.000000 | **-0.0004** | `-6.4%` | `STOP_LOSS_HIT` | $0.1088 |

> 💡 *Full granular dataset with all 2793 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
