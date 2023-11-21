# Close ALL mt4

This code is a simple and effective Forex software for quick order closure in MetaTrader 4 (mt4). It provides several functions to close orders with different criteria.

## Functionality

### CloseAllOrders()
This function closes all open orders in the current symbol and account. It iterates through all the orders from the most recent to the oldest and closes them using the `OrderClose()` function.

### CButton class
This class represents a button on the chart. It has properties such as text, position, size, color, and a clicked flag. The `Draw()` method draws the button on the chart, and the `m_clicked` flag is set to true when the button is clicked.

### OnChartEvent()
This function is called when a chart event occurs, specifically when an object is clicked. It creates two buttons, 'Close by Filter' and 'Close ALL', and draws them on the chart. It checks if either button is clicked and calls the respective function (`CloseByFilter()` or `CloseAllOrders()`) to close the orders based on the user's selection.

### CloseByFilter()
This function allows the user to close orders based on customizable profit and loss values. It iterates through all the orders and checks if the order's profit is greater than or equal to the profit value or less than or equal to the loss value. If the condition is met, it closes the order using the `OrderClose()` function.

### OnTick()
This function is called on every tick of the chart. It checks if the current time is 18:00 (6:00 PM) and calls the `CloseAllOrders()` function to close all orders. This can be used for scheduled order closure.

## Product Description

Close ALL mt4 is a simple and effective Forex software designed to provide quick order closure in MetaTrader 4. It offers several features to facilitate the closure of multiple orders with different criteria, allowing traders to efficiently manage their positions.

With Close ALL mt4, you can easily close all open orders in the current symbol and account with just one click. The software iterates through all the orders and closes them using the OrderClose function, providing a hassle-free way to clean up your trading account.

The software also offers a customizable filter function, allowing you to close orders based on specific profit and loss values. With this feature, you can set your desired profit and loss thresholds, and the software will automatically close orders that meet these criteria. This enables you to implement your own risk management strategy and take control of your trading performance.

In addition, Close ALL mt4 provides a scheduled closing option. You can set a specific time for the software to automatically close all orders, ensuring that you don't miss any important trading opportunities or leave positions open overnight.

Please note that ForexRobotEasy is not the official developer of Close ALL mt4. We merely provide this sample code to demonstrate how the product works. For detailed reviews and trading results, as well as to find the official developer of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/review-close-all-mt4-a-simple-and-effective-forex-software-for-quick-order-closure/).
