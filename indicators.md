# cTrader Indicator Examples

Example prompts for building professional cTrader indicators with Xen AI.

These examples demonstrate how to create technical indicators using plain English. Each prompt can be copied into Xen AI and customised to suit your own trading strategy.

---

## Multi-Timeframe EMA Trend Indicator

### What it builds

A professional indicator that displays the trend direction across multiple timeframes using exponential moving averages.

### Difficulty

Beginner

### Prompt

```text
Create a professional cTrader indicator named "Multi-Timeframe EMA Trend".

Display the current trend for the M5, M15, H1 and H4 timeframes using the 50 EMA and 200 EMA.

Use green for bullish trends and red for bearish trends.

Allow the EMA periods and displayed timeframes to be customised using parameters.

Follow official cTrader API best practices and keep the code modular.
```

---

## Support and Resistance Indicator

### What it builds

An indicator that automatically identifies and plots significant support and resistance levels.

### Difficulty

Beginner

### Prompt

```text
Create a professional cTrader indicator named "Dynamic Support and Resistance".

Automatically detect swing highs and swing lows and draw horizontal support and resistance levels.

Allow users to configure the swing strength, maximum levels displayed and line colours.

Only display significant price levels and keep the chart clean.

Follow official cTrader API best practices.
```

---

## Session High and Low Indicator

### What it builds

An indicator that tracks the current trading session's highest and lowest prices.

### Difficulty

Beginner

### Prompt

```text
Create a professional cTrader indicator named "Session High Low".

Display the current session high and low using horizontal lines.

Allow users to choose the trading session, line colours and line styles.

Update automatically as new highs and lows are created.

Keep the code modular and compatible with the latest cTrader API.
```

---

## Volume Heatmap Indicator

### What it builds

A visual indicator that highlights unusually high and low trading volume directly on the chart.

### Difficulty

Intermediate

### Prompt

```text
Create a professional cTrader indicator named "Volume Heatmap".

Highlight bars using different colours based on relative trading volume.

Allow users to configure the averaging period and volume thresholds.

Include a legend showing Low, Normal and High volume activity.

Use a modern Bloomberg-style colour theme and follow cTrader API best practices.
```

---

## Price Efficiency Ratio Indicator

### What it builds

An indicator that measures how efficiently price moves between two points, helping identify trending and ranging markets.

### Difficulty

Intermediate

### Prompt

```text
Create a professional cTrader indicator named "Price Efficiency Ratio".

Calculate the efficiency ratio over a configurable lookback period.

Display the indicator in a separate window with configurable trend threshold levels.

Allow users to customise colours, periods and alert levels.

Follow official cTrader API best practices and keep the code well structured.
```

---

## Tips

Describe exactly what you want the indicator to display, where it should appear, and which parameters should be configurable.

For visual indicators, describing the desired appearance, such as a Bloomberg-style dashboard or modern trading interface, often produces better results.

You can also upload a chart mock-up or screenshot for Xen AI to recreate the layout.

---

## Notes

These examples are provided for educational purposes. Always review, compile and test generated code before using it on a live trading account.
