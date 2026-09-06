# 📊 Institutional Backtest Performance Report: DOGE_USDT

> **Generated:** `2026-09-06 08:18:59 UTC` | **Engine:** `KCEX High-Fidelity Dual-Feed Simulator v1.3`

---

## ⚡ Executive Scorecard

| Performance Metric | USDT Value | INR Value (₹94.45) | % Return / Ratio |
| :--- | :--- | :--- | :--- |
| **Initial Capital** | `100.0000 USDT` | `₹9,445.00` | Baseline (100.0%) |
| **Final Balance** | `99.9530 USDT` | `₹9,440.56` | `-0.05%` |
| **Net Realized PnL** | **`-0.0470 USDT`** | **`₹-4.44`** | **`-0.05% Net ROI`** |
| **Gross Profit** | `+1.6332 USDT` | `₹154.26` | Total positive trade returns |
| **Gross Loss** | `-1.6802 USDT` | `₹158.69` | Total negative trade drawdowns |
| **Total Taker Fees Paid** | `0.000000 USDT` | `₹0.00` | `0.0000% of capital` |
| **Profit Factor** | **`0.97`** | — | Unprofitable / Needs Optimization |
| **Win / Loss Payoff** | `0.08` | — | Average Win vs Average Loss ratio |
| **Max Drawdown** | `-0.0739 USDT` | `₹6.98` | **`-0.07%` Peak-to-Trough** |
| **Win Rate** | **`92.39%`** | — | `8166 Wins / 672 Losses / 1 Scratch` |
| **Sharpe Ratio (est)** | `-0.58` | — | Annualized risk-adjusted excess return |
| **Sortino Ratio** | `-0.16` | — | Downside risk-adjusted return ratio |
| **Calmar Ratio** | `-0.64` | — | Net ROI divided by Max Drawdown |

---

## 🛠️ Complete Configuration & Settings Used

### Strategy & Market Setup
| Configuration Setting | Value | Operational Details |
| :--- | :--- | :--- |
| **Trading Pair Symbol** | `DOGE_USDT` | Base Asset: `DOGE` / Quote Asset: `USDT` |
| **Candle Timeframe** | `1m` | Dynamic candle granularity evaluated by strategy indicators |
| **Strategy Evaluated** | `STOCH_RSI` | Stochastic RSI Momentum Scalper (Preset: FAST_SCALP ; Overbought/Oversold Reversal) |
| **Strategy Preset** | `FAST_SCALP` | Configured indicator preset profile |
| **Evaluation Date Range** | `2026-07-01` → `2026-08-31` | Historical evaluation window |
| **High-Fidelity Simulation** | `DISABLED (Candle OHLC)` | Millisecond-level trade order matching & stop triggering |
| **Slippage Tolerance** | `0 ticks` (`0.00000 USDT` per fill) | Adverse fill penalty applied to entry and exit orders |

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
| **Sizing Mode** | `CONTRACTS` | Mode: `CONTRACTS`, `MULTIPLIER`, or `MIN` |
| **Trade Volume / Quantity** | `1 contract(s) (10 DOGE per trade)` | Quantity committed per trade signal |
| **Leverage Multiplier** | `75x` | Margin required = Position Notional / Leverage |
| **Starting Capital** | `100.00 USDT` | `₹9,445.00 INR` (`1 USDT = ₹94.45`) |
| **Take Profit Target** | `+2 ticks` (`+0.00002 USDT`) | Guaranteed Min-Profit TP (`entry + N*pu`) |
| **Stop Loss Rule** | `-25.0% ROE on committed margin` | Stop loss evaluation logic |

### Exchange Contract Specifications & Fees
| Specification | Value | Notes |
| :--- | :--- | :--- |
| **Fee Schedule Mode** | `ZERO` | Live KCEX API, 0.0% zero-fee pair, or manual rate |
| **Maker Fee Rate** | `0.0000%` | Rate for passive limit orders |
| **Taker Fee Rate** | `0.0000%` | Rate for aggressive market / stop triggers |
| **Contract Size (cs)** | `10.0 DOGE` | 1 contract = 10.0 underlying coin |
| **Price Unit (pu / tick)** | `1e-05` | Minimum tick increment on order book |
| **Price Precision** | `5 decimal places` | Precision formatting for quotes and orders |
| **Min Volume** | `1.0 contract(s)` | Minimum permissible order size |
| **Max Leverage** | `100x` | Maximum allowed leverage on exchange |

---

## 📈 Trade Execution & Statistical Breakdown

| Metric | Value | Context / Benchmark |
| :--- | :--- | :--- |
| **Total Trades Executed** | `8839` | Total completed trade lifecycle events |
| **Winning Trades** | `8166` | `92.39%` of total trades |
| **Losing Trades** | `672` | `7.60%` of total trades |
| **Scratch / Break-even** | `1` | `0.01%` of total trades |
| **Average Trade PnL** | `-0.0000 USDT` (`₹-0.00`) | Expected return per signal |
| **Average Winning Trade** | `+0.0002 USDT` | Average gain when trade hits TP |
| **Average Losing Trade** | `-0.0025 USDT` | Average loss when trade hits SL |
| **Largest Winning Trade** | `+0.0002 USDT (+2.1% ROE)` | Trade #1 (LONG) |
| **Largest Losing Trade** | `-0.0031 USDT (-25.1% ROE)` | Trade #7226 (LONG) |
| **Max Consecutive Wins** | `118` trades | Peak winning streak |
| **Max Consecutive Losses** | `3` trades | Peak losing streak |
| **Average Trade Duration** | `4m 20s` | Mean time from entry to exit fill |
| **Fastest Trade Fill** | `0.1s` | Trade #8839 |
| **Longest Trade In-Position** | `4h 24m 00s` | Trade #6486 |
| **Cumulative Time In Position** | `640h 28m 00s` | Total market exposure duration |

---

## 🧭 Directional Performance Analysis (LONG vs SHORT)

| Metric | LONG Trades | SHORT Trades | Combined Total |
| :--- | :--- | :--- | :--- |
| **Total Trades** | `4441` (50.2%) | `4398` (49.8%) | `8839` |
| **Wins / Losses** | `4089 W / 352 L` | `4077 W / 320 L` | `8166 W / 672 L` |
| **Win Rate** | **`92.07%`** | **`92.70%`** | **`92.39%`** |
| **Gross Profit** | `+0.8178 USDT` | `+0.8154 USDT` | `+1.6332 USDT` |
| **Gross Loss** | `-0.8851 USDT` | `-0.7951 USDT` | `-1.6802 USDT` |
| **Net Realized PnL** | **`-0.0673 USDT`** | **`+0.0203 USDT`** | **`-0.0470 USDT`** |
| **Net PnL (INR)** | `₹-6.36` | `₹+1.92` | `₹-4.44` |
| **Profit Factor** | `0.92` | `1.03` | `0.97` |

---

## 🎯 Exit Reason & Outcome Attribution

| Exit Reason Trigger | Count | % of Trades | Total PnL (USDT) | Total PnL (INR) | Win Rate | Avg Duration |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `MIN_PROFIT_TP_HIT` | `8166` | `92.4%` | `+1.6332 USDT` | `₹+154.26` | `100.0%` | `3m 24s` |
| `STOP_LOSS_HIT` | `672` | `7.6%` | `-1.6802 USDT` | `₹-158.69` | `0.0%` | `15m 47s` |
| `MANUAL_CLOSE` | `1` | `0.0%` | `+0.0000 USDT` | `₹+0.00` | `0.0%` | `0.1s` |

---

## 📜 Detailed Trade Journal

| # | Dir | Entry Time (UTC) | Exit Time (UTC) | Duration | Entry Price | Exit Price | Notional | Margin | Fee (USDT) | Net PnL (USDT) | ROE % | Exit Reason | Ending Balance |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | `LONG` | 2026-07-01 00:28:59 UTC | 2026-07-01 00:30:59 UTC | 2m 00s | `0.07182` | `0.07184` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0002 |
| 2 | `SHORT` | 2026-07-01 00:35:59 UTC | 2026-07-01 00:38:59 UTC | 3m 00s | `0.07186` | `0.07184` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0004 |
| 3 | `LONG` | 2026-07-01 00:44:59 UTC | 2026-07-01 00:52:59 UTC | 8m 00s | `0.07169` | `0.07171` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0006 |
| 4 | `SHORT` | 2026-07-01 00:54:59 UTC | 2026-07-01 01:01:59 UTC | 7m 00s | `0.07175` | `0.07173` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0008 |
| 5 | `LONG` | 2026-07-01 01:08:59 UTC | 2026-07-01 01:09:59 UTC | 1m 00s | `0.07136` | `0.07138` | $0.71 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0010 |
| 6 | `LONG` | 2026-07-01 01:14:59 UTC | 2026-07-01 01:15:59 UTC | 1m 00s | `0.07102` | `0.07104` | $0.71 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0012 |
| 7 | `SHORT` | 2026-07-01 01:18:59 UTC | 2026-07-01 01:19:59 UTC | 1m 00s | `0.07112` | `0.07110` | $0.71 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0014 |
| 8 | `SHORT` | 2026-07-01 01:22:59 UTC | 2026-07-01 01:23:59 UTC | 1m 00s | `0.07126` | `0.07124` | $0.71 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0016 |
| 9 | `SHORT` | 2026-07-01 01:32:59 UTC | 2026-07-01 01:33:59 UTC | 1m 00s | `0.07138` | `0.07136` | $0.71 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0018 |
| 10 | `SHORT` | 2026-07-01 01:43:59 UTC | 2026-07-01 01:44:59 UTC | 1m 00s | `0.07189` | `0.07187` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0020 |
| 11 | `LONG` | 2026-07-01 01:52:59 UTC | 2026-07-01 01:53:59 UTC | 1m 00s | `0.07184` | `0.07186` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0022 |
| 12 | `SHORT` | 2026-07-01 01:58:59 UTC | 2026-07-01 01:59:59 UTC | 1m 00s | `0.07184` | `0.07182` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0024 |
| 13 | `LONG` | 2026-07-01 02:03:59 UTC | 2026-07-01 02:04:59 UTC | 1m 00s | `0.07194` | `0.07196` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0026 |
| 14 | `LONG` | 2026-07-01 02:09:59 UTC | 2026-07-01 02:10:59 UTC | 1m 00s | `0.07176` | `0.07178` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0028 |
| 15 | `SHORT` | 2026-07-01 02:18:59 UTC | 2026-07-01 02:19:59 UTC | 1m 00s | `0.07202` | `0.07200` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0030 |
| 16 | `SHORT` | 2026-07-01 02:25:59 UTC | 2026-07-01 02:26:59 UTC | 1m 00s | `0.07210` | `0.07208` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0032 |
| 17 | `LONG` | 2026-07-01 02:29:59 UTC | 2026-07-01 02:30:59 UTC | 1m 00s | `0.07209` | `0.07211` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0034 |
| 18 | `LONG` | 2026-07-01 02:31:59 UTC | 2026-07-01 02:32:59 UTC | 1m 00s | `0.07206` | `0.07208` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0036 |
| 19 | `LONG` | 2026-07-01 02:35:59 UTC | 2026-07-01 02:38:59 UTC | 3m 00s | `0.07214` | `0.07216` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0038 |
| 20 | `SHORT` | 2026-07-01 02:47:59 UTC | 2026-07-01 02:48:59 UTC | 1m 00s | `0.07191` | `0.07189` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0040 |
| 21 | `LONG` | 2026-07-01 02:51:59 UTC | 2026-07-01 02:53:59 UTC | 2m 00s | `0.07194` | `0.07196` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0042 |
| 22 | `SHORT` | 2026-07-01 02:58:59 UTC | 2026-07-01 03:06:59 UTC | 8m 00s | `0.07195` | `0.07219` | $0.72 | $0.01 | $0.000000 | **-0.0024** | `-25.0%` | `STOP_LOSS_HIT` | $100.0018 |
| 23 | `SHORT` | 2026-07-01 03:09:59 UTC | 2026-07-01 03:10:59 UTC | 1m 00s | `0.07209` | `0.07207` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0020 |
| 24 | `LONG` | 2026-07-01 03:19:59 UTC | 2026-07-01 03:21:59 UTC | 2m 00s | `0.07186` | `0.07188` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0022 |
| 25 | `LONG` | 2026-07-01 03:23:59 UTC | 2026-07-01 03:25:59 UTC | 2m 00s | `0.07192` | `0.07194` | $0.72 | $0.01 | $0.000000 | **+0.0002** | `+2.1%` | `MIN_PROFIT_TP_HIT` | $100.0024 |
| ... | ... | *(8789 intermediate trades logged in full .csv report)* | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 8815 | `SHORT` | 2026-08-30 21:11:59 UTC | 2026-08-30 21:13:59 UTC | 2m 00s | `0.08459` | `0.08457` | $0.85 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9543 |
| 8816 | `SHORT` | 2026-08-30 21:15:59 UTC | 2026-08-30 21:16:59 UTC | 1m 00s | `0.08460` | `0.08458` | $0.85 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9545 |
| 8817 | `LONG` | 2026-08-30 21:25:59 UTC | 2026-08-30 21:26:59 UTC | 1m 00s | `0.08446` | `0.08448` | $0.84 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9547 |
| 8818 | `SHORT` | 2026-08-30 21:36:59 UTC | 2026-08-30 21:37:59 UTC | 1m 00s | `0.08480` | `0.08478` | $0.85 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9549 |
| 8819 | `LONG` | 2026-08-30 21:45:59 UTC | 2026-08-30 21:46:59 UTC | 1m 00s | `0.08438` | `0.08440` | $0.84 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9551 |
| 8820 | `LONG` | 2026-08-30 21:49:59 UTC | 2026-08-30 21:50:59 UTC | 1m 00s | `0.08435` | `0.08437` | $0.84 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9553 |
| 8821 | `SHORT` | 2026-08-30 21:55:59 UTC | 2026-08-30 21:57:59 UTC | 2m 00s | `0.08446` | `0.08444` | $0.84 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9555 |
| 8822 | `SHORT` | 2026-08-30 21:59:59 UTC | 2026-08-30 22:00:59 UTC | 1m 00s | `0.08458` | `0.08456` | $0.85 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9557 |
| 8823 | `SHORT` | 2026-08-30 22:05:59 UTC | 2026-08-30 22:06:59 UTC | 1m 00s | `0.08465` | `0.08463` | $0.85 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9559 |
| 8824 | `LONG` | 2026-08-30 22:13:59 UTC | 2026-08-30 22:14:59 UTC | 1m 00s | `0.08423` | `0.08425` | $0.84 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9561 |
| 8825 | `LONG` | 2026-08-30 22:19:59 UTC | 2026-08-30 22:20:59 UTC | 1m 00s | `0.08424` | `0.08426` | $0.84 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9563 |
| 8826 | `SHORT` | 2026-08-30 22:22:59 UTC | 2026-08-30 22:24:59 UTC | 2m 00s | `0.08385` | `0.08383` | $0.84 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9565 |
| 8827 | `LONG` | 2026-08-30 22:29:59 UTC | 2026-08-30 22:30:59 UTC | 1m 00s | `0.08371` | `0.08343` | $0.84 | $0.01 | $0.000000 | **-0.0028** | `-25.1%` | `STOP_LOSS_HIT` | $99.9537 |
| 8828 | `SHORT` | 2026-08-30 22:35:59 UTC | 2026-08-30 22:36:59 UTC | 1m 00s | `0.08358` | `0.08356` | $0.84 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9539 |
| 8829 | `SHORT` | 2026-08-30 22:43:59 UTC | 2026-08-30 22:44:59 UTC | 1m 00s | `0.08370` | `0.08368` | $0.84 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9541 |
| 8830 | `LONG` | 2026-08-30 22:53:59 UTC | 2026-08-30 22:54:59 UTC | 1m 00s | `0.08359` | `0.08361` | $0.84 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9543 |
| 8831 | `SHORT` | 2026-08-30 23:00:59 UTC | 2026-08-30 23:04:59 UTC | 4m 00s | `0.08339` | `0.08337` | $0.83 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9545 |
| 8832 | `SHORT` | 2026-08-30 23:15:59 UTC | 2026-08-30 23:16:59 UTC | 1m 00s | `0.08333` | `0.08331` | $0.83 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9547 |
| 8833 | `LONG` | 2026-08-30 23:27:59 UTC | 2026-08-30 23:28:59 UTC | 1m 00s | `0.08245` | `0.08247` | $0.82 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9549 |
| 8834 | `LONG` | 2026-08-30 23:31:59 UTC | 2026-08-30 23:35:59 UTC | 4m 00s | `0.08215` | `0.08188` | $0.82 | $0.01 | $0.000000 | **-0.0027** | `-24.7%` | `STOP_LOSS_HIT` | $99.9522 |
| 8835 | `SHORT` | 2026-08-30 23:36:59 UTC | 2026-08-30 23:37:59 UTC | 1m 00s | `0.08197` | `0.08195` | $0.82 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9524 |
| 8836 | `LONG` | 2026-08-30 23:42:59 UTC | 2026-08-30 23:43:59 UTC | 1m 00s | `0.08150` | `0.08152` | $0.82 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9526 |
| 8837 | `LONG` | 2026-08-30 23:50:59 UTC | 2026-08-30 23:51:59 UTC | 1m 00s | `0.08156` | `0.08158` | $0.82 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9528 |
| 8838 | `SHORT` | 2026-08-30 23:54:59 UTC | 2026-08-30 23:55:59 UTC | 1m 00s | `0.08179` | `0.08177` | $0.82 | $0.01 | $0.000000 | **+0.0002** | `+1.8%` | `MIN_PROFIT_TP_HIT` | $99.9530 |
| 8839 | `SHORT` | 2026-08-31 00:00:59 UTC | 2026-08-31 00:00:59 UTC | 0.1s | `0.08182` | `0.08182` | $0.82 | $0.01 | $0.000000 | **+0.0000** | `+0.0%` | `MANUAL_CLOSE` | $99.9530 |

> 💡 *Full granular dataset with all 8839 trades is stored in the accompanying `trades.csv` and `trades.jsonl` artifacts.*
