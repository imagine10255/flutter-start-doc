# 問題

```text
flutter: NoSuchMethodError: Closure call with mismatched arguments: function 'DepositService.uploadWebBankDetail' 
Receiver: Closure: (String) => Future from Function 'uploadWebBankDetail': static. 
Tried calling: DepositService.uploadWebBankDetail() 
Found: DepositService.uploadWebBankDetail(String) => Future<UploadWebBankPlusDetailRes>
```

DepositService.uploadWebBankDetail 這個方法 遺失必填參數

