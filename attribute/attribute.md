---
description: 進階容器額外屬性
---

# Decoration

### Decoration Class介绍

Decoration是個窗口小部件\(widget\)，可以在子widget的繪製前後對其進行裝飾，Decoration的定義如下：

```text
DecoratedBox({Key key, @required Decoration decoration, DecorationPosition position: DecorationPosition.background, Widget child })
```

*  `decoration` : 裝飾器接口，Decoration是個抽象接口，BoxDecoration是它其一個具體實現類，Decoration裝飾器的繪製最終會由BoxPainter來完成，實現一個Decoration裝飾器可以通過createBoxPainter方法來獲取一個BoxPainter，最終通過BoxPainter來進行繪製。
*  `position`: 是個枚舉類型，用來控制裝飾器在哪裡繪製，取值有background跟foreground，前者代表是在背景繪製，後者是在前景繪製

### BoxDecoration介绍

BoxDecoration是Decoration的一個實現類，BoxDecoration提供了背景顏色、邊框、陰影、圓角、顏色漸變、形狀等等裝飾能力，BoxDecoration的定義如下

```dart
BoxDecoration({
  Color color,
  DecorationImage image,
  BoxBorder border,
  BorderRadiusGeometry borderRadius, 
  List<BoxShadow> boxShadow,
  Gradient gradient,
  BlendMode backgroundBlendMode,
  BoxShape shape = BoxShape.rectangle, 
})
```

*  `color` ： 背景颜色
*  `image` ：背景圖片，會在背景顏色上面
*  `border` ：邊框，會畫在背景顏色上
*  `borderRadius` ： 邊框圓角
*  `boxShadow` ：背景陰影
*  `gradient` ： 漸變顏色
*  `backgroundBlendMode` ： 背景混合模式
*  `shape` ： 形狀

### **可使用該屬性的元件**

* Container
* TextField, TextFormField

