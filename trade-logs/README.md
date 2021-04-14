# Trade Logs
Firestore trade-logs collection data model

```
{
  type: `STOCK_${tradeType}`,
  userId: userId,
  stockName: stockData.name,
  orderValue,
  quantity: qtyUserCanPurchase,
  price: stockData.price,
  timestamp: +Date.now()
}
```