---
description: List<> 遞迴
---

# List&lt;dynamic&gt; map

### 使用方法

```dart
List<String> data = ['a','b','c']


// 一般
data.map((row) { 
  return Text('${row}');
}
// >> a 
// >> b
// >> c

// 取得 index 方法
data.asMap().entries.map((entry) {
  int index = entry.key;
  String row = entry.value;
 
  return Text('${index} -> ${row}');
}

// >> 0 -> a 
// >> 1 -> b
// >> 2 -> c
```

 

