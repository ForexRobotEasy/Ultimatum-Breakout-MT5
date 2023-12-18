# Ultimatum Breakout MT5

This code is a sample implementation of the Ultimatum Breakout strategy for MetaTrader 5 (MT5). It is intended to be used as a template for creating an Expert Advisor (EA) that automatically trades based on breakout levels.

## Input Parameters

- **BreakoutPeriod**: Specifies the number of bars used to calculate the breakout level.
- **StopLoss**: Sets the stop loss level in points.
- **TakeProfit**: Sets the take profit level in points.

## Global Variables

- **lastHigh**: Stores the highest price of the previous bar.
- **lastLow**: Stores the lowest price of the previous bar.

## Expert Initialization Function

The `OnInit()` function is called once during the initialization of the EA. It calculates the last high and low values based on historical price data.

## Expert Deinitialization Function

The `OnDeinit()` function is called when the EA is being removed from the chart or when the terminal is shut down. It can be used for any necessary cleanup tasks.

## Expert Start Function

The `OnTick()` function is called on each tick of the chart. It calculates the breakout level as the average of the last high and low prices. If the current Ask price is above the breakout level, a BuyStop pending order is placed with the stop loss and take profit levels calculated based on the input parameters. If the current Bid price is below the breakout level, a SellStop pending order is placed with the corresponding stop loss and take profit levels.

The function also updates the last high and low values based on the current price.

## Product Description

Ultimatum Breakout MT5 is a powerful and customizable Expert Advisor that trades breakouts in the forex market. It is designed to take advantage of price movements after a consolidation period, aiming to capture profitable trades with minimal risk.

This EA uses a breakout strategy, which identifies key levels of support and resistance and enters trades when the price breaks out of these levels. It incorporates intelligent risk management with adjustable stop loss and take profit levels, allowing you to control your risk and maximize your potential profits.

Key Features:

- Breakout period: Allows you to specify the number of bars used to calculate the breakout level.
- Stop loss and take profit: Set your desired levels of risk and reward.
- Fully customizable: Adapt the EA to your trading preferences and market conditions.
- Easy to use: No complicated settings or parameters to worry about.
- Real-time monitoring: Track the performance of the EA with detailed reviews and trading results.

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that demonstrates how the Ultimatum Breakout strategy can be implemented. To find the official developer of this product, please refer to the MQL5 website.

For detailed reviews and trading results of this product, please visit [https://forexroboteasy.com/forex-robot-review/ultimatum-breakout-mt5-review-real-results-and-download-of-ea-golden-cat-mt4-5](https://forexroboteasy.com/forex-robot-review/ultimatum-breakout-mt5-review-real-results-and-download-of-ea-golden-cat-mt4-5)
