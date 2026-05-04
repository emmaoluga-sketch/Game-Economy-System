# 🧱 System Architecture

## Flow:

1. Player performs action (buy, trade, earn)
2. Client sends request to server
3. Server validates request
4. CurrencyManager updates balance
5. DataManager saves data
6. TransactionLogger logs event

---

## Modules

### CurrencyManager
Handles:
- AddCurrency
- RemoveCurrency
- GetBalance

### TradeManager
Handles:
- Trade requests
- Trade validation
- Item exchange

### Validation
Handles:
- Anti-exploit checks
- Input validation

### TransactionLogger
Handles:
- Logging transactions
- Debug tracking
