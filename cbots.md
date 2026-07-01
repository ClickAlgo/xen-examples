# cBot Automated Trading Examples

Example prompts for building automated trading strategies (cBots) with Xen AI.

These prompts are designed to help you create complete trading systems using plain English. Each example generates a fully automated cTrader cBot that can be modified and extended.

---

## Moving Average Crossover Strategy

### What it builds

A simple automated trading system based on moving average crossovers.

### Difficulty

Beginner

### Prompt

```text id="cb1"
Create a cTrader cBot named "Moving Average Crossover Strategy".

The bot should use a fast and slow moving average to generate trade signals.

Enter a BUY trade when the fast moving average crosses above the slow moving average.

Enter a SELL trade when the fast moving average crosses below the slow moving average.

Allow users to configure moving average periods, lot size, stop loss and take profit.

Include a filter to prevent multiple open positions in the same direction.

Follow official cTrader API best practices and ensure the code is clean and modular.
```

---

## Breakout Trading Strategy

### What it builds

A volatility breakout cBot that trades when price breaks recent highs or lows.

### Difficulty

Beginner

### Prompt

```text id="cb2"
Create a cTrader cBot named "Breakout Trading Strategy".

The bot should detect breakouts of the highest high and lowest low over a configurable lookback period.

Enter a BUY trade when price breaks above the highest high.

Enter a SELL trade when price breaks below the lowest low.

Include stop loss and take profit inputs.

Add a session filter so trades only occur during active trading hours.

Ensure the bot avoids duplicate entries on the same breakout.
```

---

## RSI Mean Reversion Strategy

### What it builds

A mean reversion cBot using RSI overbought and oversold conditions.

### Difficulty

Beginner

### Prompt

```text id="cb3"
Create a cTrader cBot named "RSI Mean Reversion Strategy".

Use RSI with a configurable period.

Enter a BUY trade when RSI falls below the oversold level.

Enter a SELL trade when RSI rises above the overbought level.

Include stop loss, take profit and position sizing inputs.

Add a trend filter using a moving average to avoid trading against strong trends.

Ensure only one trade per signal condition.
```

---

## Grid Recovery Strategy

### What it builds

A grid-based trading system that adds positions at predefined price intervals.

### Difficulty

Intermediate

### Prompt

```text id="cb4"
Create a cTrader cBot named "Grid Recovery Strategy".

Place an initial trade and then place additional orders at fixed pip intervals in the same direction if price moves against the position.

Include inputs for grid step size, maximum number of grid levels, lot scaling and overall risk limit.

Add a global stop loss to close all positions if maximum drawdown is reached.

Ensure the bot prevents overexposure and respects account risk limits.
```

---

## Trend Pullback Strategy

### What it builds

A trend-following system that enters trades on pullbacks within an established trend.

### Difficulty

Intermediate

### Prompt

```text id="cb5"
Create a cTrader cBot named "Trend Pullback Strategy".

Identify trend direction using a moving average or market structure.

Enter BUY trades during pullbacks in an uptrend and SELL trades during pullbacks in a downtrend.

Use a configurable pullback threshold for entry signals.

Include stop loss below recent swing lows or above swing highs.

Allow configuration of trade session filters and risk per trade.

Ensure the bot avoids overtrading and respects trend conditions.
```

---

## Tips

Clearly define:

* Entry conditions
* Exit conditions
* Risk rules
* Filters (trend, session, volatility)
* Position limits

The more structured the description, the more reliable the generated cBot.

---

## Notes

These examples are for educational purposes. Always test generated cBots in a demo environment before using them on live accounts.
