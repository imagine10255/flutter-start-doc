---
description: 直列上到下排列方式的 Widget
---

# Column, Row

該 Widget 相等於 Web flex-direction column, Row

### Column

![Column &#x6392;&#x5217;&#x65B9;&#x5411;](../.gitbook/assets/image%20%281%29.png)

### 使用方式

```dart
Column(
  mainAxisAlignment: MainAxisAlignment.center,
  mainAxisSize: MainAxisSize.min,
  children: [
    Text('上'),
    Text('下'),
  ],
),
```

{% hint style="info" %}
如果你單純是列表項目, 請使用 ListView  
如果你是列表項目, 並且非常多, 請使用 ListView.builder
{% endhint %}

### Row 

![Row &#x6392;&#x5217;&#x65B9;&#x5411;](../.gitbook/assets/image.png)

### 使用方式

```dart
Row(
  mainAxisAlignment: MainAxisAlignment.center,
  mainAxisSize: MainAxisSize.min,
  children: [
    Text('左'),
    Text('右'),
  ],
),
```

