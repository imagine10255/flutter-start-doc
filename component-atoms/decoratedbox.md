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

* `decoration` : 裝飾器接口，Decoration是個抽象接口，BoxDecoration是它其一個具體實現類，Decoration裝飾器的繪製最終會由BoxPainter來完成，實現一個Decoration裝飾器可以通過createBoxPainter方法來獲取一個BoxPainter，最終通過BoxPainter來進行繪製。
*  `position`: 是個枚舉類型，用來控制裝飾器在哪裡繪製，取值有background跟foreground，前者代表是在背景繪製，後者是在前景繪製

### 參考連結

{% embed url="https://book.flutterchina.club/chapter5/decoratedbox.html" %}



