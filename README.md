# Miliarto Forex Robot

This is the code for the Miliarto Forex Robot, developed by the Forex Robot Easy Team. Please note that ForexRobotEasy is not the official developer of this product. We are only showcasing a sample code that can work as described in the official product.

For detailed reviews and trading results of this product, please visit [this link](https://forexroboteasy.com/forex-robot-review/miliarto-forex-software-review-of-ea-with-bollinger-bands/).

## Description

The Miliarto Forex Robot is an Expert Advisor (EA) designed to trade in the Forex market. It uses the Moving Average (MA) and Bollinger Bands indicators to determine buy and sell signals. The EA has various input parameters that can be customized according to the trader's preferences.

### Input Parameters

- **MA_Method**: Moving Average method (default: MODE_SMA)
- **MA_Period**: Moving Average period (default: 14)
- **MA_Price**: Moving Average applied price (default: PRICE_CLOSE)
- **BB_Period**: Bollinger Bands period (default: 20)
- **BB_Deviation**: Bollinger Bands deviation (default: 2.0)
- **TP_in_Pips**: Take Profit in pips (default: 50)
- **SL_in_Pips**: Stop Loss in pips (default: 25)
- **Use_Martingale**: Enable Martingale setup (default: true)

### Global Variables

- **Lots**: Initial lot size (default: 0.01)
- **Martingale_Factor**: Martingale factor (default: 2.0)

## How It Works

The Miliarto Forex Robot uses the MA and Bollinger Bands indicators to generate buy and sell signals. 

1. On each tick, the EA calculates the current MA value and the upper and lower Bollinger Bands values.
2. If the previous candle's close is below the MA and the current candle's close is above the MA and above the lower Bollinger Band, a buy signal is generated.
3. If the previous candle's close is above the MA and the current candle's close is below the MA and below the upper Bollinger Band, a sell signal is generated.
4. For each signal, the EA sets the stop loss (SL) and take profit (TP) levels based on the input parameters.
5. If the Martingale setup is enabled, the lot size is increased by the Martingale factor after each trade.

Please note that this code is a simplified version and may require further modification and optimization for actual trading.

## Disclaimer

Please note that ForexRobotEasy is not the official developer of this product. We are only showcasing a sample code that can work as described in the official product. To find the official developer of this product, please visit MQL5.

For detailed reviews and trading results of this product, please visit [this link](https://forexroboteasy.com/forex-robot-review/miliarto-forex-software-review-of-ea-with-bollinger-bands/).
