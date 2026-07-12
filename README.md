# TradingView Pine Script Collection

A collection of Pine Script v5 indicators, strategies, and libraries.

## Structure

```
├── indicators/
│   ├── EMA_Crossover.pine       # EMA crossover signals with alerts
│   └── RSI_Divergence.pine      # RSI divergence detection
├── strategies/
│   └── EMA_Crossover_Strategy.pine  # Full strategy with SL/TP backtesting
└── libraries/
    └── Utils.pine               # Shared utility functions
```

## How to Use

1. Open [TradingView](https://www.tradingview.com) and go to the **Pine Script Editor** (bottom panel)
2. Paste the contents of any `.pine` file
3. Click **Add to chart**

## Indicators

### EMA Crossover
Plots fast/slow EMAs and marks crossover points with shapes and background colour.
- Configurable fast/slow lengths and source
- Built-in alerts for bullish and bearish crosses

### RSI Divergence
Detects classic bullish and bearish RSI divergences using pivot points.
- Configurable RSI length, overbought/oversold levels, and pivot lookback
- Alerts on divergence signals

## Strategies

### EMA Crossover Strategy
Backtestable strategy based on the EMA crossover signal.
- Optional ATR-based stop loss and take profit
- Configurable risk % per trade
- Commission included (0.1% default)

## Libraries

### Utils
Reusable Pine Script library with helper functions:
- `atr_stop()` — ATR-based stop distance
- `is_consolidating()` — Consolidation detection
- `normalize()` — 0-100 normalisation
- `gradient_color()` — Red/yellow/green gradient colour
