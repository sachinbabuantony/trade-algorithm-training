# HTF Pivots and CHoCH Indicator

Welcome to the **HTF Pivots and CHoCH Indicator** project! This Pine Script-based TradingView strategy is designed to help traders identify high-timeframe pivots, market structures, and CHoCH (Change of Character) points. It also incorporates automated trade execution logic with risk-reward settings for a complete trading system.

## Features

### 1. High-Timeframe Pivots
- Identifies high-timeframe pivot highs and lows using customizable settings.
- Uses `request.security` to fetch pivot data from higher timeframes.
- Dynamically draws pivot lines on the chart with real-time updates.

### 2. Market Structure Detection
- Detects bullish and bearish market structures (e.g., BOS - Break of Structure, CHoCH - Change of Character).
- Highlights key bullish and bearish zones with user-defined colors.
- Optionally displays support and resistance levels as dashed lines.

### 3. Trade Execution Logic
- Implements buy and sell conditions based on market structure breaks.
- Uses a configurable **Risk:Reward** ratio to calculate stop-loss and take-profit levels.
- Automatically cancels untriggered orders after a specified number of candles.
- Displays entry, stop-loss, and take-profit levels visually on the chart.

### 4. Dashboard
- Provides a summary of bullish and bearish structure statistics.
- Displays the percentage of market structures that align with fractals.
- Customizable location and text size for the dashboard.

### 5. Visualization
- Clearly plots pivot lines, market structure labels, and trade zones.
- Highlights breakout points for support and resistance levels.
- Uses real-time updates to ensure the chart reflects the current market conditions.

## How It Works

### High-Timeframe Pivots
- The script calculates pivot highs and lows using a lookback period (`Pivot Lookback`) on a higher timeframe (`Pivot Timeframe`).
- These pivots are stored and plotted dynamically on the chart.

### Market Structure
- Identifies bullish and bearish fractals based on a lookback period (`BOS/CHoCH Indicator Settings`).
- Tracks breakouts of previous pivot levels to determine BOS or CHoCH.
- Labels the chart with "BOS" or "CHoCH" to indicate the type of breakout.

### Trade Execution
- Trades are triggered when specific conditions (e.g., BOS, CHoCH) are met.
- Entry price, stop-loss, and take-profit levels are calculated and plotted.
- If an order is not triggered within a set number of candles, it is automatically canceled.

### Dashboard
- Displays the ratio of bullish and bearish structures that align with fractals.
- Provides a quick overview of market structure statistics.

## Settings and Inputs

### HTF Pivot Settings
- **Pivot Timeframe**: The timeframe for calculating high-timeframe pivots (e.g., 15 minutes, 1 hour).
- **Pivot Lookback**: Number of candles to look back for pivot calculations.

### BOS/CHoCH Indicator Settings
- **Length**: Lookback period for detecting market structures.
- **Bullish Structures**: Toggle to show bullish structure labels and lines.
- **Bearish Structures**: Toggle to show bearish structure labels and lines.
- **Support**: Toggle to show support levels.
- **Resistance**: Toggle to show resistance levels.

### Strategy Settings
- **Risk:Reward**: Set the desired risk-to-reward ratio for trades.
- **SL Lookback Candles**: Number of candles to use for calculating stop-loss levels.
- **Order Cancel Candles**: Number of candles after which untriggered orders are canceled.
- **Enable Trades**: Toggle to enable or disable trade execution.

### Dashboard Settings
- **Show Dashboard**: Toggle to display the dashboard.
- **Location**: Set the position of the dashboard (e.g., Top Right, Bottom Left).
- **Size**: Set the text size of the dashboard (e.g., Tiny, Small, Normal).

## How to Use

1. Copy and paste the script into TradingView's Pine Editor.
2. Adjust the settings according to your trading preferences.
3. Add the script to your chart and observe the plotted pivots, market structures, and trade zones.
4. Enable trade execution if you want to automate trading based on the strategy.

## Disclaimer
This script is provided for educational purposes only. Use it at your own risk. Always test strategies on a demo account before applying them to live trades.

## License
This project is licensed under the [Mozilla Public License 2.0](https://mozilla.org/MPL/2.0/).

## Author
- **Sachin Babu Antony**  
Feel free to contribute or raise issues to improve the script!

---
Happy Trading!
