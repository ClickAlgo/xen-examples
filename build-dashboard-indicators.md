# cTrader Dashboard Indicator Example

Example prompt for building a professional cTrader dashboard indicator with Xen AI.

This example creates a chart-based account statistics dashboard using cTrader controls. It is designed as a simple first version that can later be expanded with more statistics, sections, alerts, or visual styling.

---

## Trading Statistics Dashboard

### What it builds

A cTrader indicator named **Trading Statistics Dashboard** that displays key account statistics in a modern dashboard panel on the chart.

### Difficulty

Beginner

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

- Use a clean professional appearance like a Bloomberg dashboard
- Automatically resize based on the content.
- Allow the dashboard position to be changed using parameters (Top Left, Top Right, Bottom Left, Bottom Right).
- Display labels in one column and values in a second aligned column.
- Refresh automatically whenever account information changes.
- Follow official cTrader API best practices.
- Keep the code well structured and modular so additional dashboard sections can easily be added later.
```

### Expected result

A clean account statistics dashboard displayed on the cTrader chart, with labels and values aligned in two columns. The first version focuses on layout, structure, and live account statistics rather than trading logic.

### Suggested follow-up prompts

```text
Add daily profit and loss, weekly profit and loss, and monthly profit and loss to the dashboard.
```

```text
Add colour highlighting so positive values appear green and negative values appear red.
```

```text
Add a collapsible section for open position statistics.
```

---

## Tips

When creating dashboard indicators, describe the layout clearly. Include the position, columns, values, colours, refresh behaviour, and whether the dashboard should be an indicator, cBot, plugin, or trading panel.

For more complex dashboards, upload a mock-up image to Xen AI and describe how the layout should behave.

---

## Notes

This example is for educational use. Always build and test generated code in cTrader before using it on a live trading account.
