---
description: '垂直, 水平排列方式的 Widget'
---

# Column, Row



## Column

![Column &#x6392;&#x5217;&#x65B9;&#x5411;](../.gitbook/assets/image%20%281%29.png)

### 使用方法

```dart
Column(
  mainAxisAlignment: MainAxisAlignment.center,
  crossAxisAlignment: CrossAxisAlignment.start,
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
如果你是畫面超出, 請使用 [SingleChildScrollView](single-child-scroll-view.md)
{% endhint %}



### 屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| [MainAxisAlignment](../attribute-class/main-axis-alignment.md) | mainAxisAlignment | 垂直對齊方式 |  |
| [CrossAxisAlignment](../attribute-class/cross-axis-alignment.md) | crossAxisAlignment | 水平對齊方式 |  |
| [MainAxisSize](../attribute-class/main-axis-size.md) | mainAxisSize |  |  |
| Widget | child | 內容 |  |

## Row 

![Row &#x6392;&#x5217;&#x65B9;&#x5411;](../.gitbook/assets/image.png)

### 使用方法

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

### 屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| [MainAxisAlignment](../attribute-class/main-axis-alignment.md) | mainAxisAlignment | 水平對齊方式 |  |
| [CrossAxisAlignment](../attribute-class/cross-axis-alignment.md) | crossAxisAlignment | 垂直對齊方式 |  |
| [MainAxisSize](../attribute-class/main-axis-size.md) | mainAxisSize |  |  |
| Widget | child | 內容 |  |

## 

