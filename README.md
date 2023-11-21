# Gold Dragon MT4

Gold Dragon MT4 is a professional Forex trading software designed specifically for trading gold (XAUUSD) on the H1 timeframe. This Expert Advisor uses advanced trend analysis algorithms to identify trading opportunities and execute trades automatically.

## Developer

This Expert Advisor is developed by Forex Robot Easy Team.

## Website

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/review-gold-dragon-mt4-professional-forex-trading-software-for-gold-xauusd-h1-trading/).

## Global Variables

- `stopLoss`: Stop Loss in pips, default value is 50.
- `takeProfit`: Take Profit in pips, default value is 100.

## Expert Advisor Function Definitions

### `CalculateTrendPower()`

This function calculates the trend power of daily candles. Advanced trend analysis algorithms can be added here. It returns the calculated trend power.

### `OpenBuyTrade()`

This function opens a buy trade. It uses the `CalculateTrendPower()` function to determine the trend power. The Stop Loss and Take Profit levels for the trade are set based on the global variables `stopLoss` and `takeProfit`. The buy trade is executed with the specified Stop Loss and Take Profit levels.

### `OpenSellTrade()`

This function opens a sell trade. It uses the `CalculateTrendPower()` function to determine the trend power. The Stop Loss and Take Profit levels for the trade are set based on the global variables `stopLoss` and `takeProfit`. The sell trade is executed with the specified Stop Loss and Take Profit levels.

### `CloseAllTrades()`

This function closes all open trades.

## Expert Advisor Initialization Function

### `OnInit()`

This function is called once when the EA is loaded. Initialization code can be added here. It returns `INIT_SUCCEEDED` to indicate successful initialization.

## Expert Advisor Start Function

### `OnTick()`

This function is called for every tick. It checks for trading opportunities and opens or closes trades accordingly. If there are any open trades, it closes them using the `CloseAllTrades()` function. If there are no open trades, it calculates the trend power using the `CalculateTrendPower()` function and opens buy or sell trades based on the trend power.

## Expert Advisor Deinitialization Function

### `OnDeinit(const int reason)`

This function is called once when the EA is unloaded. Deinitialization code can be added here.

## Expert Advisor Program

### `OnStart()`

This is the entry point of the Expert Advisor program. It starts the EA by calling the `OnTick()` function. The EA runs on every tick.

Please note that Forex Robot Easy is not the official developer of this product. This code is provided as a sample that can work similarly to the described product. To find the official developer of this product, please use MQL5.
