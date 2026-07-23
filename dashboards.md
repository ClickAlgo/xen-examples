# cTrader Dashboard Indicator Examples

Example prompts for building professional cTrader dashboard indicators with Xen AI.

These examples are designed for traders who want visual account, risk, trade, market, and performance dashboards inside cTrader without manually writing C# code.

Dashboard prompts usually work better when you describe the visual style clearly. For example, asking for a **Bloomberg-style dashboard** often produces a cleaner, more professional layout with stronger spacing, alignment, typography, and colour structure.

---

## Example 1 - Trading Statistics Dashboard

### What it builds

A cTrader indicator named **Trading Statistics Dashboard** that displays key account statistics in a modern dashboard panel on the chart.

### Difficulty

Beginner

### Suggested theme

Bloomberg-style dark dashboard.

### Prompt

```text
Create a professional cTrader indicator named "Trading Statistics Dashboard".

The indicator should display a modern dashboard in the top right corner of the chart using cTrader controls.

The dashboard should be designed so additional statistics can easily be added in future versions.

For this first version, focus only on creating the dashboard layout and displaying the following account statistics:

- Account Balance
- Account Equity
- Free Margin
- Margin Level
- Open Positions
- Pending Orders

Requirements:

- Use a clean professional appearance like a Bloomberg dashboard.
- Automatically resize based on the content.
- Allow the dashboard position to be changed using parameters (Top Left, Top Right, Bottom Left, Bottom Right).
- Display labels in one column and values in a second aligned column.
- Refresh automatically whenever account information changes.
- Follow official cTrader API best practices.
- Keep the code well structured and modular so additional dashboard sections can easily be added later.
```

### Expected result

A clean account statistics dashboard displayed on the cTrader chart, with labels and values aligned in two columns. The first version focuses on layout, structure, and live account statistics rather than trading logic.

---

## Example 2 - Account Risk Dashboard

### What it builds

A cTrader indicator dashboard that displays account exposure, margin usage, and basic risk information for open positions.

### Difficulty

Intermediate

### Suggested theme

Professional risk desk dashboard with dark panels and clear warning colours.

### Prompt

```text
Create a professional cTrader indicator named "Account Risk Dashboard".

The indicator should display a modern risk dashboard on the chart using cTrader controls.

The dashboard should focus on account risk and exposure from current open positions.

Display the following information:

- Account Balance
- Account Equity
- Used Margin
- Free Margin
- Margin Level
- Number of Open Positions
- Total Open Position Volume
- Total Unrealised Profit or Loss
- Largest Losing Position
- Largest Winning Position

Requirements:

- Use a clean professional risk desk appearance with a dark background.
- Use green text for positive profit values and red text for negative profit values.
- Use amber or orange warning text when margin level falls below a configurable warning level.
- Allow the dashboard position to be changed using parameters (Top Left, Top Right, Bottom Left, Bottom Right).
- Add input parameters for font size, dashboard opacity, and margin warning level.
- Display labels in one column and values in a second aligned column.
- Refresh automatically when account or position information changes.
- Do not place, modify, or close trades. This must be an indicator only.
- Follow official cTrader API best practices.
- Keep the code modular so additional risk metrics can easily be added later.
```

### Expected result

A risk-focused account dashboard that helps the user monitor live exposure and margin pressure without executing trades.

---

## Example 3 - Open Trades Dashboard

### What it builds

A cTrader indicator dashboard that summarises open trades by symbol, direction, volume, and profit or loss.

### Difficulty

Intermediate

### Suggested theme

Trading desk blotter style.

### Prompt

```text
Create a professional cTrader indicator named "Open Trades Dashboard".

The indicator should display a trading desk style dashboard showing current open trade information.

Display a compact table with the following columns:

- Symbol
- Direction
- Volume
- Entry Price
- Current Price
- Net Profit
- Pips
- Trade Age

Requirements:

- Use a clean trading desk blotter style layout.
- Display buy positions in green and sell positions in red.
- Display profitable trades in green and losing trades in red.
- Allow the dashboard position to be changed using parameters (Top Left, Top Right, Bottom Left, Bottom Right).
- Add input parameters for maximum rows, font size, and dashboard opacity.
- If there are more open positions than the maximum rows, show a summary row such as "Additional positions hidden".
- Automatically resize based on the visible rows.
- Refresh automatically as prices and open position information change.
- Do not place, modify, or close trades. This must be an indicator only.
- Follow official cTrader API best practices.
- Keep the code well structured so more trade columns can be added later.
```

### Expected result

A compact open trades dashboard that shows live trade information directly on the chart.

---

## Example 4 - Daily Performance Dashboard

### What it builds

A cTrader indicator dashboard that displays daily trading performance, including closed profit or loss and current floating profit or loss.

### Difficulty

Intermediate

### Suggested theme

Modern performance analytics dashboard.

### Prompt

```text
Create a professional cTrader indicator named "Daily Performance Dashboard".

The indicator should display a modern performance analytics dashboard on the chart.

The dashboard should focus on today's trading activity and performance.

Display the following information:

- Today's Closed Profit or Loss
- Today's Floating Profit or Loss
- Today's Total Profit or Loss
- Number of Trades Closed Today
- Winning Trades Today
- Losing Trades Today
- Win Rate Today
- Average Profit per Closed Trade
- Best Trade Today
- Worst Trade Today

Requirements:

- Use a clean modern analytics dashboard appearance.
- Use green for positive values and red for negative values.
- Use a clear header showing the current trading date.
- Allow the dashboard position to be changed using parameters (Top Left, Top Right, Bottom Left, Bottom Right).
- Add input parameters for font size, dashboard opacity, and whether to include floating profit or loss.
- Display labels in one column and values in a second aligned column.
- Refresh automatically when account, position, or trade history information changes.
- Do not place, modify, or close trades. This must be an indicator only.
- Follow official cTrader API best practices.
- Keep the code modular so weekly and monthly performance sections can be added later.
```

### Expected result

A daily trading performance dashboard that helps the user monitor closed and floating results for the current day.

---

## Example 5 - Multi-Symbol Market Dashboard

### What it builds

A cTrader indicator dashboard that monitors several symbols and displays market status information in one panel.

### Difficulty

Intermediate

### Suggested theme

Bloomberg-style market monitor.

### Prompt

```text
Create a professional cTrader indicator named "Multi-Symbol Market Dashboard".

The indicator should display a Bloomberg-style market monitor dashboard on the chart using cTrader controls.

The dashboard should allow the user to monitor several symbols from one chart.

Display a table with the following columns:

- Symbol
- Bid
- Ask
- Spread
- Daily Change
- ATR
- Trend Status

Use the following logic:

- Calculate ATR using a configurable ATR period.
- Determine Trend Status using a configurable fast EMA and slow EMA.
- If fast EMA is above slow EMA, show Bullish.
- If fast EMA is below slow EMA, show Bearish.
- If the values are very close, show Neutral.

Requirements:

- Allow the user to enter symbols as a comma-separated list.
- Use a clean Bloomberg-style dark dashboard appearance.
- Use green for Bullish and positive daily change.
- Use red for Bearish and negative daily change.
- Use grey or neutral styling for Neutral status.
- Allow the dashboard position to be changed using parameters (Top Left, Top Right, Bottom Left, Bottom Right).
- Add input parameters for symbol list, ATR period, fast EMA period, slow EMA period, font size, and dashboard opacity.
- Automatically resize based on the number of symbols.
- Refresh automatically as market prices update.
- Do not place, modify, or close trades. This must be an indicator only.
- Follow official cTrader API best practices.
- Keep the code modular so more market columns can easily be added later.
```

### Expected result

A multi-symbol market dashboard that gives the user a quick overview of spread, volatility, daily movement, and trend status.

---

## Example 6 - Multi Timeframe Trend Matrix Dashboard

### What it builds

A cTrader indicator dashboard that analyses trend direction and strength across multiple timeframes using EMA calculations, weighted scoring, and alignment analysis.

### Difficulty

Advanced

### Suggested theme

Professional dark trading desk dashboard.

### Prompt

```text
Create a new cTrader Algo indicator project named "Multi Timeframe Trend Matrix".

Implement only the initial dashboard layout and multi-timeframe data foundation in this iteration.

Create a fixed chart dashboard using cTrader controls with a clean, compact, professional dark trading-desk appearance.

Display a title bar reading:

Multi Timeframe Trend Matrix

Create one row for each of these timeframes:

- M1
- M5
- M15
- M30
- H1
- H4
- Daily
- Weekly
- Monthly

Create the following columns:

- Timeframe
- Trend
- Strength

For this first iteration:

- Load market-series data for the current chart symbol for every listed timeframe.
- Display "Pending" in the Trend column.
- Display "--" in the Strength column.
- Do not calculate trend direction, strength, weighted scores or alignment yet.
- Show a clear neutral message instead of failing if data for a timeframe is unavailable.

Add parameters for:

- Dashboard position: Top Left, Top Right, Bottom Left or Bottom Right
- Font size, default 12
- Dashboard opacity

Use Top Right as the default dashboard position.

This indicator must only analyse and display information. It must not place, modify or close trades.

Keep the implementation modular so calculations can be added in later iterations.

Return one complete, compile-ready C# file. Stop after completing this iteration.

---

## Theme Ideas for Dashboard Prompts

You can improve dashboard results by describing the visual style clearly.

Examples:

```text
Use a clean professional appearance like a Bloomberg dashboard.
```

```text
Use a modern dark trading desk style with compact aligned rows.
```

```text
Use a clean institutional risk dashboard style with warning colours.
```

```text
Use a minimal light theme with subtle borders and clear spacing.
```

```text
Use a glassmorphism-style dashboard with semi-transparent panels.
```

For most trading tools, a Bloomberg-style or trading desk style dashboard is usually the safest choice because it encourages a professional, compact, information-dense layout.

---

## Suggested Follow-Up Prompts

```text
Add colour highlighting so positive values appear green and negative values appear red.
```

```text
Add a collapsible section for advanced statistics.
```

```text
Make the dashboard draggable while keeping the selected dashboard position as the default starting location.
```

```text
Add input parameters for panel background colour, border colour, and text colour.
```

```text
Add a compact mode that shows fewer rows and uses smaller spacing.
```

---

## Tips

When creating dashboard indicators, describe the layout clearly. Include the dashboard position, columns, values, colours, refresh behaviour, and whether the dashboard should be an indicator, cBot, plugin, or trading panel.

For more complex dashboards, upload a mock-up image to Xen AI and describe how the layout should behave.

DRAGGABLE PANEL

To enable a draggable panel on the chart, the user MUST write exactly:

"make the panel draggable on the chart"

No additional text, requirements, or explanations should be included.

This phrase is used as a direct RAG key to inject draggable panel behaviour into the generated code.
If the phrase is missing, the panel must remain fixed using the selected position parameter (TopLeft, TopRight, BottomLeft, BottomRight).

---

## Notes

These examples are for educational use. Always build and test generated code in cTrader before using it on a live trading account.
