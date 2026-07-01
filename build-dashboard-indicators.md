# cTrader Dashboard Indicator Examples

Example prompts for building cTrader dashboard indicators with Xen AI.

These prompts are designed for traders who want visual dashboards, market status panels, account summaries, or multi-symbol indicator displays inside cTrader without manually writing C# code.

---

## Example 1 - Multi-Symbol Trend Dashboard

### What it builds

A cTrader indicator dashboard that displays the current trend direction across multiple symbols using moving averages.

### Difficulty

Beginner

### Prompt

```text
Build a cTrader indicator dashboard that shows the trend direction for multiple symbols.

Requirements:

- Display the following symbols: EURUSD, GBPUSD, USDJPY, XAUUSD and US30.
- Use a 50-period EMA and 200-period EMA to determine trend direction.
- If EMA 50 is above EMA 200, show Bullish.
- If EMA 50 is below EMA 200, show Bearish.
- Display each symbol in a clean dashboard table.
- Columns should include Symbol, EMA 50, EMA 200 and Trend.
- Use green text for Bullish and red text for Bearish.
- Place the dashboard in the top-left corner of the chart.
- Add input parameters for the EMA periods, symbols list and dashboard position.
- Make the code compatible with the latest cTrader Automate API.
```

### Expected result

A visual dashboard indicator showing several symbols and their current EMA trend status.

---

## Example 2 - RSI Market Strength Dashboard

### What it builds

A dashboard indicator showing RSI values and overbought/oversold status across multiple symbols.

### Difficulty

Beginner

### Prompt

```text
Build a cTrader dashboard indicator that monitors RSI values across multiple symbols.

Requirements:

- Use RSI period 14 by default.
- Allow the user to enter a comma-separated symbol list.
- Display Symbol, RSI Value and Status.
- If RSI is above 70, show Overbought.
- If RSI is below 30, show Oversold.
- Otherwise show Neutral.
- Use red for Overbought, green for Oversold and gray for Neutral.
- Refresh the dashboard on each bar.
- Add input parameters for RSI period, overbought level, oversold level, symbols and dashboard position.
- Keep the dashboard simple, clean and readable.
```

### Expected result

A compact RSI dashboard for quickly checking market conditions across selected symbols.

---

## Example 3 - Account Risk Dashboard

### What it builds

A cTrader indicator that displays account and open-position risk information directly on the chart.

### Difficulty

Intermediate

### Prompt

```text
Build a cTrader dashboard indicator that displays account risk information.

Requirements:

- Show account balance.
- Show account equity.
- Show free margin.
- Show margin level.
- Show number of open positions.
- Show total unrealised profit or loss.
- Show total volume of open positions.
- Display the dashboard as a clean panel on the chart.
- Use green for positive profit and red for negative profit.
- Add input parameters for dashboard position, font size and panel opacity.
- Update the dashboard in real time.
- Do not place trades. This must be an indicator only.
```

### Expected result

A non-trading dashboard for monitoring account exposure and open-position status.

---

## Tips for Better Dashboard Prompts

* State whether you want an indicator, cBot, plugin, dashboard or trading panel.
* Describe every column or value you want displayed.
* Mention colours only when they matter.
* Include where the dashboard should appear on the chart.
* Say whether it should update on every tick or every bar.
* Upload a mock-up image if the layout is important.

---

## Related Videos

Add YouTube links here when available.

```text
Video: Build a Multi-Symbol Trend Dashboard with Xen AI
Link: https://youtube.com/your-video-link
```

---

## Notes

These examples are for educational use. Always test generated code in cTrader before using it on a live trading account.
