# Iterative cTrader Dashboard Build Example

This example shows how to divide a complex cTrader dashboard into small implementation prompts for Xen AI.

Submit each prompt separately. Build and test the generated code before using the next prompt.

---

# Prompt 1: Create the Visual Foundation

## COPY PROMPT 1 FROM HERE

```text
Create a new cTrader dashboard indicator named "Trading Performance Dashboard".

Implement only the initial visual design and user settings in this iteration.

Visual design:

- Create a modern, dark, Bloomberg-style dashboard.
- Use consistent padding, spacing, alignment, and typography.
- Include a title bar displaying "Trading Performance Dashboard".

User settings:

- Allow the dashboard to be anchored to Top Left, Top Right, Bottom Left, or Bottom Right.
- Use Top Right as the default position.
- Add a font-size setting with a default value of 13 pixels.

For this iteration, the panel body must contain only:

Dashboard initialised...

Do not add account information, trading statistics, position statistics, controls, or other features yet.

Return one complete, compile-ready C# file. Stop after completing this iteration.
```

## END OF PROMPT 1

Build and test Prompt 1 before continuing.

---

# Prompt 2: Add Live Account Information

## COPY PROMPT 2 FROM HERE

```text
Update the existing Trading Performance Dashboard created in the previous step.

Replace the placeholder content with a live account-information section.

Display:

- Account Balance
- Account Equity
- Floating Profit/Loss
- Current Drawdown in the account deposit currency
- Current Drawdown as a percentage

Definitions:

- Floating Profit/Loss is the combined unrealised net profit or loss across all currently open positions.
- Current Drawdown is the difference between Account Balance and Account Equity when Equity is below Balance.
- Drawdown Percentage = ((Balance - Equity) / Balance) × 100.
- If Equity is greater than or equal to Balance, display zero drawdown.
- If Balance is zero, display zero for the drawdown percentage.

Requirements:

- Update all values in real time.
- Display positive values in green.
- Display negative values in red.
- Display neutral and zero values using the standard text colour.
- Preserve the existing title, visual design, position setting, font-size setting, spacing, and layout.
- Add only the account-information section.
- Do not add trading-performance or open-position statistics yet.
- Do not redesign or refactor unrelated code.

Return one complete, compile-ready C# file. Stop after completing this iteration.
```

## END OF PROMPT 2

Build and test Prompt 2 before continuing.

---

# Prompt 3: Add Trading Performance Statistics

## COPY PROMPT 3 FROM HERE

```text
Update the existing Trading Performance Dashboard created in the previous steps.

Add a Trading Performance section displaying:

- Today's Profit/Loss
- This Week's Profit/Loss
- Total Trades Today
- Win Rate
- Average Win
- Average Loss
- Profit Factor

Definitions:

- Use completed trades only.
- Exclude open positions from all calculations.
- Today's Profit/Loss is the combined net profit of trades completed during the current calendar day.
- Total Trades Today is the number of trades completed during the current calendar day.
- This Week's Profit/Loss is the combined net profit of trades completed from Monday at 00:00 to the current time.
- Use the indicator's configured time zone for day and week boundaries.
- Win Rate uses all available completed trades.
- A winning trade has net profit greater than zero.
- A losing trade has net profit less than zero.
- A break-even trade has net profit equal to zero and must not count as a win or loss.
- Win Rate = Winning Trades / (Winning Trades + Losing Trades) × 100.
- Average Win is the average net profit of all winning trades.
- Average Loss is the average absolute net loss of all losing trades.
- Profit Factor = Total Net Profit from Winning Trades / Absolute Total Net Loss from Losing Trades.
- Display zero when a calculation has no qualifying trades or would require division by zero.

Requirements:

- Calculate the statistics efficiently.
- Preserve all existing account information, settings, visual design, and working behaviour.
- Add only the Trading Performance section.
- Do not add open-position statistics yet.
- Do not add unrelated statistics.
- Do not redesign or refactor unrelated code.

Return one complete, compile-ready C# file. Stop after completing this iteration.
```

## END OF PROMPT 3

Build and test Prompt 3 before continuing.

---

# Prompt 4: Add Open-Position Statistics

## COPY PROMPT 4 FROM HERE

```text
Update the existing Trading Performance Dashboard created in the previous steps.

Add an Open Positions section displaying:

- Buy Positions
- Sell Positions
- Total Open Positions
- Floating Profit/Loss
- Total Volume
- Total Exposure

Definitions:

- Buy Positions is the number of currently open buy positions.
- Sell Positions is the number of currently open sell positions.
- Total Open Positions is the combined number of open buy and sell positions.
- Floating Profit/Loss is the combined unrealised net profit or loss of all open positions.
- Total Volume is the combined volume of all open positions.
- Total Exposure is the gross notional exposure of all open positions, converted to the account deposit currency before aggregation.
- Sum the absolute notional exposure of each position.
- Do not offset buy exposure against sell exposure.
- When there are no open positions, display zero for every value in this section.

Requirements:

- Update the values in real time as positions and market prices change.
- Preserve all existing account information, performance statistics, settings, layout, visual design, and working behaviour.
- Add only the Open Positions section.
- Do not add unrelated statistics or controls.
- Do not redesign or refactor unrelated code.

Return one complete, compile-ready C# file. Stop after completing this iteration.
```

## END OF PROMPT 4

Build and test Prompt 4.

---

# Testing Order

1. Copy and submit Prompt 1 to Xen.
2. Build and test the result.
3. Copy and submit Prompt 2 only after Prompt 1 works.
4. Continue with Prompt 3 and then Prompt 4.
5. If an iteration fails, fix it before using the next prompt.

Do not submit all four prompts to Xen together.
