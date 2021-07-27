---
description: 簡化版的 Container (單純只提供 decorated 屬性的 Widget)
---

# DecoratedBox

### 使用方法

```dart
DecoratedBox(
  decoration: BoxDecoration(
    gradient: LinearGradient(colors:[Colors.red,Colors.orange[700]]), //背景渐变
    borderRadius: BorderRadius.circular(3.0), //3像素圆角
    boxShadow: [ //阴影
      BoxShadow(
        color:Colors.black54,
        offset: Offset(2.0,2.0),
        blurRadius: 4.0
      )
    ]
  ),
  child: Padding(padding: EdgeInsets.symmetric(horizontal: 80.0, vertical: 18.0),
    child: Text("Login", style: TextStyle(color: Colors.white),),
  )
)
```

### 屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| [Decoration](../attribute-class/decoration.md) | decoration | 前景背景裝飾 |  |
| DecorationPosition | position | 類型 | DecorationPosition.background |
| Widget | child | 內容 |  |

* position:
  * DecorationPosition.background 背景
  * DecorationPosition.foreground 前景

### 參考連結

{% embed url="https://book.flutterchina.club/chapter5/decoratedbox.html" %}



