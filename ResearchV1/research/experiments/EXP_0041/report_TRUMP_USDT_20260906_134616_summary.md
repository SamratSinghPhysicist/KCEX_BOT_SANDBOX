# 📊 Institutional Backtest Performance Report: TRUMP_USDT

> **Generated:** `2026-09-06 08:16:17 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `0.0700 USDT` | `₹6.61` | Baseline (100.0%) |
| **Final Balance** | `0.0896 USDT` | `₹8.46` | `+28.00%` |
| **Net Realized PnL** | **`+0.0196 USDT`** | **`₹+1.85`** | **`+28.00% Net ROI`** |
| **Gross Profit** | `+0.6588 USDT` | `₹62.22` | Total positive trade returns |
| **Gross Loss** | `-0.6392 USDT` | `₹60.37` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`1.03`** | — | Profitable |
| **Win / Loss Payoff** | `1.00` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0184 USDT` | `₹1.74` | **`-19.41%` Peak-to-Trough** |
| **Win Rate** | **`50.76%`** | — | `1647 Wins / 1598 Losses / 0 Scratch` |
| **Sharpe Ratio (est)** | `1.36` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `1.36` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `1.44` | — | Net ROI divided by Max Drawdown |

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
| **Total Trades Executed** | `3245` | Total completed trade lifecycle events |
| **Winning Trades** | `1647` | `50.76%` of total trades |
| **Losing Trades** | `1598` | `49.24%` of total trades |
| **Scratch / Break-even** | `0` | `0.00%` of total trades |
| **Average Trade PnL** | `+0.0000 USDT` (`₹+0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0004 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0004 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0004 USDT (+9.6% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0004 USDT (-9.6% ROE)` | Trade #4 (LONG) |
| **Max Consecutive Wins** | `9` trades | Peak winning streak |
| **Max Consecutive Losses** | `8` trades | Peak losing streak |
| **Average Trade Duration** | `2m 56s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #787 |
| **Longest Trade In-Position** | `48m 43s` | Trade #146 |
| **Cumulative Time In Position** | `159h 10m 17s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `1629` (50.2%) | `1616` (49.8%) | `3245` |
| **Wins / Losses** | `796 W / 833 L` | `851 W / 765 L` | `1647 W / 1598 L` |
| **Win Rate** | **`48.86%`** | **`52.66%`** | **`50.76%`** |
| **Gross Profit** | `+0.3184 USDT` | `+0.3404 USDT` | `+0.6588 USDT` |
| **Gross Loss** | `-0.3332 USDT` | `-0.3060 USDT` | `-0.6392 USDT` |
| **Net Realized PnL** | **`-0.0148 USDT`** | **`+0.0344 USDT`** | **`+0.0196 USDT`** |
| **Net PnL (INR)** | `₹-1.40` | `₹+3.25` | `₹+1.85` |
| **Profit Factor** | `0.96` | `1.11` | `1.03` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `1647` | `50.8%` | `+0.6588 USDT` | `₹+62.22` | `100.0%` | `2m 56s` |
| `STOP_LOSS_HIT` | `1598` | `49.2%` | `-0.6392 USDT` | `₹-60.37` | `0.0%` | `2m 56s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-25 00:27:59 UTC | 2026-07-25 00:31:24 UTC | 3m 24s | `1.561` | `1.563` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0704 |
| 2 | `SHORT` | 2026-07-25 00:36:59 UTC | 2026-07-25 00:42:01 UTC | 5m 01s | `1.563` | `1.561` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0708 |
| 3 | `LONG` | 2026-07-25 00:44:59 UTC | 2026-07-25 00:46:48 UTC | 1m 48s | `1.560` | `1.562` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 4 | `LONG` | 2026-07-25 00:47:59 UTC | 2026-07-25 00:48:15 UTC | 15.0s | `1.564` | `1.562` | $0.31 | $0.00 | $0.000000 | **-0.0004** | `-9.6%` | `STOP_LOSS_HIT` | $0.0708 |
| 5 | `SHORT` | 2026-07-25 00:51:59 UTC | 2026-07-25 00:53:51 UTC | 1m 51s | `1.562` | `1.560` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0712 |
| 6 | `SHORT` | 2026-07-25 01:00:59 UTC | 2026-07-25 01:04:37 UTC | 3m 37s | `1.567` | `1.565` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0716 |
| 7 | `LONG` | 2026-07-25 01:13:59 UTC | 2026-07-25 01:16:13 UTC | 2m 13s | `1.561` | `1.563` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0720 |
| 8 | `SHORT` | 2026-07-25 01:31:59 UTC | 2026-07-25 01:36:41 UTC | 4m 41s | `1.558` | `1.560` | $0.31 | $0.00 | $0.000000 | **-0.0004** | `-9.6%` | `STOP_LOSS_HIT` | $0.0716 |
| 9 | `LONG` | 2026-07-25 01:56:59 UTC | 2026-07-25 01:57:54 UTC | 54.9s | `1.556` | `1.558` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0720 |
| 10 | `LONG` | 2026-07-25 02:04:59 UTC | 2026-07-25 02:06:42 UTC | 1m 42s | `1.552` | `1.554` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.7%` | `MIN_PROFIT_TP_HIT` | $0.0724 |
| 11 | `SHORT` | 2026-07-25 02:10:59 UTC | 2026-07-25 02:14:00 UTC | 3m 00s | `1.557` | `1.555` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0728 |
| 12 | `LONG` | 2026-07-25 02:19:59 UTC | 2026-07-25 02:22:43 UTC | 2m 43s | `1.556` | `1.554` | $0.31 | $0.00 | $0.000000 | **-0.0004** | `-9.6%` | `STOP_LOSS_HIT` | $0.0724 |
| 13 | `LONG` | 2026-07-25 02:26:59 UTC | 2026-07-25 02:29:02 UTC | 2m 02s | `1.555` | `1.557` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0728 |
| 14 | `SHORT` | 2026-07-25 02:32:59 UTC | 2026-07-25 02:38:16 UTC | 5m 16s | `1.555` | `1.557` | $0.31 | $0.00 | $0.000000 | **-0.0004** | `-9.6%` | `STOP_LOSS_HIT` | $0.0724 |
| 15 | `SHORT` | 2026-07-25 02:45:59 UTC | 2026-07-25 02:48:47 UTC | 2m 47s | `1.558` | `1.556` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0728 |
| 16 | `LONG` | 2026-07-25 02:51:59 UTC | 2026-07-25 02:52:49 UTC | 49.1s | `1.555` | `1.557` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0732 |
| 17 | `SHORT` | 2026-07-25 02:57:59 UTC | 2026-07-25 03:00:12 UTC | 2m 12s | `1.559` | `1.561` | $0.31 | $0.00 | $0.000000 | **-0.0004** | `-9.6%` | `STOP_LOSS_HIT` | $0.0728 |
| 18 | `SHORT` | 2026-07-25 03:11:59 UTC | 2026-07-25 03:13:00 UTC | 1m 00s | `1.566` | `1.568` | $0.31 | $0.00 | $0.000000 | **-0.0004** | `-9.6%` | `STOP_LOSS_HIT` | $0.0724 |
| 19 | `LONG` | 2026-07-25 03:22:59 UTC | 2026-07-25 03:26:01 UTC | 3m 01s | `1.569` | `1.571` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0728 |
| 20 | `LONG` | 2026-07-25 03:34:59 UTC | 2026-07-25 03:38:16 UTC | 3m 16s | `1.570` | `1.568` | $0.31 | $0.00 | $0.000000 | **-0.0004** | `-9.6%` | `STOP_LOSS_HIT` | $0.0724 |
| 21 | `LONG` | 2026-07-25 03:52:59 UTC | 2026-07-25 03:57:14 UTC | 4m 14s | `1.565` | `1.567` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.6%` | `MIN_PROFIT_TP_HIT` | $0.0728 |
| 22 | `SHORT` | 2026-07-25 03:59:59 UTC | 2026-07-25 04:03:42 UTC | 3m 42s | `1.566` | `1.568` | $0.31 | $0.00 | $0.000000 | **-0.0004** | `-9.6%` | `STOP_LOSS_HIT` | $0.0724 |
| 23 | `SHORT` | 2026-07-25 04:12:59 UTC | 2026-07-25 04:14:08 UTC | 1m 08s | `1.570` | `1.572` | $0.31 | $0.00 | $0.000000 | **-0.0004** | `-9.6%` | `STOP_LOSS_HIT` | $0.0720 |
| 24 | `SHORT` | 2026-07-25 04:20:59 UTC | 2026-07-25 04:25:22 UTC | 4m 22s | `1.574` | `1.576` | $0.31 | $0.00 | $0.000000 | **-0.0004** | `-9.5%` | `STOP_LOSS_HIT` | $0.0716 |
| 25 | `LONG` | 2026-07-25 04:29:59 UTC | 2026-07-25 04:32:47 UTC | 2m 47s | `1.573` | `1.575` | $0.31 | $0.00 | $0.000000 | **+0.0004** | `+9.5%` | `MIN_PROFIT_TP_HIT` | $0.0720 |
| ... | ... | *(3195 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 3221 | `LONG` | 2026-08-14 20:49:59 UTC | 2026-08-14 20:51:14 UTC | 1m 14s | `1.454` | `1.452` | $0.29 | $0.00 | $0.000000 | **-0.0004** | `-10.3%` | `STOP_LOSS_HIT` | $0.0896 |
| 3222 | `LONG` | 2026-08-14 20:59:59 UTC | 2026-08-14 21:00:11 UTC | 11.8s | `1.451` | `1.449` | $0.29 | $0.00 | $0.000000 | **-0.0004** | `-10.3%` | `STOP_LOSS_HIT` | $0.0892 |
| 3223 | `SHORT` | 2026-08-14 21:04:59 UTC | 2026-08-14 21:05:34 UTC | 34.8s | `1.447` | `1.449` | $0.29 | $0.00 | $0.000000 | **-0.0004** | `-10.4%` | `STOP_LOSS_HIT` | $0.0888 |
| 3224 | `LONG` | 2026-08-14 21:12:59 UTC | 2026-08-14 21:13:00 UTC | 0.3s | `1.448` | `1.446` | $0.29 | $0.00 | $0.000000 | **-0.0004** | `-10.4%` | `STOP_LOSS_HIT` | $0.0884 |
| 3225 | `LONG` | 2026-08-14 21:23:59 UTC | 2026-08-14 21:26:11 UTC | 2m 11s | `1.437` | `1.435` | $0.29 | $0.00 | $0.000000 | **-0.0004** | `-10.4%` | `STOP_LOSS_HIT` | $0.0880 |
| 3226 | `SHORT` | 2026-08-14 21:31:59 UTC | 2026-08-14 21:33:36 UTC | 1m 36s | `1.438` | `1.436` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.4%` | `MIN_PROFIT_TP_HIT` | $0.0884 |
| 3227 | `LONG` | 2026-08-14 21:42:59 UTC | 2026-08-14 21:44:12 UTC | 1m 12s | `1.431` | `1.429` | $0.29 | $0.00 | $0.000000 | **-0.0004** | `-10.5%` | `STOP_LOSS_HIT` | $0.0880 |
| 3228 | `SHORT` | 2026-08-14 21:46:59 UTC | 2026-08-14 21:47:01 UTC | 1.4s | `1.427` | `1.429` | $0.29 | $0.00 | $0.000000 | **-0.0004** | `-10.5%` | `STOP_LOSS_HIT` | $0.0876 |
| 3229 | `SHORT` | 2026-08-14 21:53:59 UTC | 2026-08-14 21:54:26 UTC | 26.1s | `1.428` | `1.426` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0880 |
| 3230 | `LONG` | 2026-08-14 21:58:59 UTC | 2026-08-14 22:01:27 UTC | 2m 27s | `1.430` | `1.432` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0884 |
| 3231 | `SHORT` | 2026-08-14 22:05:59 UTC | 2026-08-14 22:06:40 UTC | 40.9s | `1.430` | `1.428` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0888 |
| 3232 | `LONG` | 2026-08-14 22:10:59 UTC | 2026-08-14 22:12:05 UTC | 1m 05s | `1.429` | `1.431` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0892 |
| 3233 | `LONG` | 2026-08-14 22:22:59 UTC | 2026-08-14 22:23:15 UTC | 15.0s | `1.423` | `1.421` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.5%` | `STOP_LOSS_HIT` | $0.0888 |
| 3234 | `SHORT` | 2026-08-14 22:27:59 UTC | 2026-08-14 22:28:17 UTC | 17.8s | `1.422` | `1.420` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0892 |
| 3235 | `SHORT` | 2026-08-14 22:38:59 UTC | 2026-08-14 22:42:05 UTC | 3m 05s | `1.422` | `1.424` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.5%` | `STOP_LOSS_HIT` | $0.0888 |
| 3236 | `SHORT` | 2026-08-14 22:44:59 UTC | 2026-08-14 22:47:56 UTC | 2m 56s | `1.421` | `1.423` | $0.28 | $0.00 | $0.000000 | **-0.0004** | `-10.6%` | `STOP_LOSS_HIT` | $0.0884 |
| 3237 | `LONG` | 2026-08-14 22:57:59 UTC | 2026-08-14 23:01:43 UTC | 3m 43s | `1.423` | `1.425` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0888 |
| 3238 | `SHORT` | 2026-08-14 23:03:59 UTC | 2026-08-14 23:08:38 UTC | 4m 38s | `1.424` | `1.422` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0892 |
| 3239 | `LONG` | 2026-08-14 23:11:59 UTC | 2026-08-14 23:15:10 UTC | 3m 10s | `1.424` | `1.426` | $0.28 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0896 |
| 3240 | `SHORT` | 2026-08-14 23:18:59 UTC | 2026-08-14 23:24:36 UTC | 5m 36s | `1.426` | `1.428` | $0.29 | $0.00 | $0.000000 | **-0.0004** | `-10.5%` | `STOP_LOSS_HIT` | $0.0892 |
| 3241 | `SHORT` | 2026-08-14 23:28:59 UTC | 2026-08-14 23:30:03 UTC | 1m 03s | `1.429` | `1.427` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0896 |
| 3242 | `LONG` | 2026-08-14 23:34:59 UTC | 2026-08-14 23:37:33 UTC | 2m 33s | `1.427` | `1.429` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0900 |
| 3243 | `SHORT` | 2026-08-14 23:44:59 UTC | 2026-08-14 23:51:47 UTC | 6m 47s | `1.433` | `1.431` | $0.29 | $0.00 | $0.000000 | **+0.0004** | `+10.5%` | `MIN_PROFIT_TP_HIT` | $0.0904 |
| 3244 | `LONG` | 2026-08-14 23:52:59 UTC | 2026-08-14 23:53:21 UTC | 21.8s | `1.433` | `1.431` | $0.29 | $0.00 | $0.000000 | **-0.0004** | `-10.5%` | `STOP_LOSS_HIT` | $0.0900 |
| 3245 | `LONG` | 2026-08-14 23:57:59 UTC | 2026-08-14 23:59:18 UTC | 1m 18s | `1.432` | `1.430` | $0.29 | $0.00 | $0.000000 | **-0.0004** | `-10.5%` | `STOP_LOSS_HIT` | $0.0896 |

> 💡 *Full granular dataset with all 3245 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
