# Saga Base



```dart
fetchWalletAmount({required FetchWalletAmountAction action}) sync* {
  // 最少3秒才結束
  yield All({
    #request: Call(WalletService.getWalletAmount, result: result),
    #delay: delay(Duration(seconds: 3)),
  });
}
```

 

