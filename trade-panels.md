# cTrader Trading Panel Examples

Example prompts for building interactive cTrader trading panels with Xen AI.

These prompts are designed for creating manual trading interfaces with buy/sell buttons, position controls and live account information. Each example can be copied into Xen AI and customised.

---

## Basic Buy Sell Panel

### What it builds

A simple trading panel with Buy and Sell buttons for manual execution.

### Difficulty

Beginner

### Prompt

```text id="tp1"
Create a cTrader trading panel named "Basic Buy Sell Panel".

The panel should include two buttons: BUY and SELL.

When clicked, BUY opens a market buy order and SELL opens a market sell order.

Include inputs for lot size, stop loss and take profit.

Display current spread and account balance on the panel.

Ensure only one position per direction is allowed.

Follow official cTrader API best practices and use a clean, modern layout.
```

---

## Risk Controlled Trading Panel

### What it builds

A manual trading panel with built-in risk controls.

### Difficulty

Beginner

### Prompt

```text id="tp2"
Create a cTrader trading panel named "Risk Controlled Panel".

Include BUY and SELL buttons for manual trading.

Add inputs for risk per trade (percentage), stop loss in pips, and take profit in pips.

Calculate position size automatically based on account balance and risk settings.

Display live account equity, margin level and open positions.

Prevent trades if risk exceeds user-defined limits.

Ensure the panel is clean, professional and easy to use.
```

---

## Multi-Position Management Panel

### What it builds

A panel for managing open positions, including closing and modifying trades.

### Difficulty

Intermediate

### Prompt

```text id="tp3"
Create a cTrader trading panel named "Position Management Panel".

Display all open positions with symbol, volume, entry price and profit/loss.

Include buttons to close individual positions or close all positions.

Allow users to modify stop loss and take profit directly from the panel.

Show total floating profit and account exposure.

Update all values in real time.

Follow official cTrader API best practices and ensure a modular design.
```

---

## Advanced Trading Terminal Panel

### What it builds

A full-featured trading terminal with execution and account monitoring.

### Difficulty

Advanced

### Prompt

```text id="tp4"
Create a cTrader trading panel named "Advanced Trading Terminal".

Include BUY and SELL buttons with market execution.

Add pending order controls (Buy Limit, Sell Limit, Buy Stop, Sell Stop).

Display account balance, equity, margin level and free margin.

Include risk management inputs for lot sizing, stop loss and take profit.

Show active positions and allow quick closing.

Design the panel with a Bloomberg-style professional layout.

Ensure all components are modular and extendable for future features.
```

---

## Session-Based Trading Panel

### What it builds

A trading panel that only allows trading during specific market sessions.

### Difficulty

Intermediate

### Prompt

```text id="tp5"
Create a cTrader trading panel named "Session Trading Panel".

Include BUY and SELL buttons for manual trading.

Allow trading only during selected sessions (London, New York, Asia).

Display current session status on the panel.

Include risk controls for lot size, stop loss and take profit.

Show spread and volatility indicator.

Disable trading buttons outside active session hours.

Ensure the panel updates in real time and follows cTrader API best practices.
```

---

## Tips

When designing trading panels, clearly define:

* Button actions (BUY, SELL, CLOSE, etc.)
* Risk controls (lot size, % risk, SL/TP)
* Live account data display
* Restrictions (session filters, max trades)
* Layout style (clean, Bloomberg-style)

The more precise the UI description, the better the generated panel.

DRAGGABLE PANEL REQUIREMENT

If you want a panel or dashboard to be draggable on the chart, you MUST explicitly include the phrase:

"make the panel draggable on the chart" ** DO THIS AS A STANDALONE SEPARATE REQUEST.

This will trigger Xen RAG to inject draggable panel behaviour automatically.

If this is not included, the default behaviour will be a fixed-position panel using the selected position parameter (TopLeft, TopRight, BottomLeft, BottomRight).

---

## Notes

These examples are for educational purposes. Always test generated trading panels in a demo environment before using them in live trading.
