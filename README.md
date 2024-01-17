# SigmaSpikes ReadMe

This code is for the SigmaSpikes indicator created by irdoj75 for the MetaTrader 4 (MT4) platform. It is a reliable non-repaint forex software. 

## Developer's Site
You can find more information about this indicator on the [developer's site](https://forexroboteasy.com/forex-robot-review/sigmaspikes-mt4-review-reliable-non-repaint-forex-software/). Please note that ForexRobotEasy is not the official developer of this product. We only provide this code as a sample that can work as described in the product.

## Development
This code was developed by the Forex Robot Easy Team.

## Indicator Inputs
- `IndicatorPeriod`: The period used for calculating the indicator values (default: 14)
- `IndicatorMethod`: The moving average method used for the indicator calculation (default: Simple Moving Average)

## Trade Inputs
- `LotSize`: The lot size used for trading (default: 0.01)
- `StopLoss`: The stop loss level in pips (default: 50)
- `TakeProfit`: The take profit level in pips (default: 100)

## Global Variables
- `buffer[]`: An array to store the calculated indicator values
- `lastBar`: The value of the last completed bar

## Indicator Initialization
The `OnInit()` function is called when the indicator is initialized. It sets up the indicator buffers and label, and calculates the initial indicator values. The `SetIndexBuffer()` function is used to set the indicator buffer. The `IndicatorSetString()` function is used to set the indicator label. The indicator values are calculated using the `CalculateIndicator()` function.

## Indicator Calculation
The `CalculateIndicator()` function calculates the indicator values based on the specified period and method. It calculates the simple moving average of the close prices for the specified period. The result is returned as the indicator value for the current index.

## Trading Function
The `OnTick()` function is called on every tick. It checks if a new bar has formed and if so, it compares the current and previous indicator values. If the current value is greater than the previous value, a buy order is placed. If the current value is less than the previous value, a sell order is placed. The order parameters are set based on the input values. The `OrderSend()` function is used to send the order. If the order is placed successfully, a success message is printed. Otherwise, an error message is printed.

## Product Description
SigmaSpikes is a reliable non-repaint forex software for the MetaTrader 4 (MT4) platform. It uses a simple moving average indicator with customizable period and method to generate trading signals. 

Key Features:
- Accurate and reliable signals
- Customizable period and method for the indicator
- Automatic buy and sell order placement
- Adjustable lot size, stop loss, and take profit levels

SigmaSpikes is designed to help traders make informed trading decisions and execute trades automatically. It is suitable for both beginner and experienced traders. 

Please note that ForexRobotEasy is not the official developer of this product. We only provide this code as a sample that can work as described in the product. To find the official developer of this product, please refer to the [developer's site](https://forexroboteasy.com/forex-robot-review/sigmaspikes-mt4-review-reliable-non-repaint-forex-software/).
