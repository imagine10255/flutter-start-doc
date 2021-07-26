---
description: 最基礎的容器 類似於Web 的 div
---

# Container

### 使用方法

```dart
Container(
  width: 100,
  height: 100,
  padding: EdgeInsets.all(12),
  margin: EdgeInsets.all(12),
  alignment: Alignment.centerLeft,
  clipBehavior: Clip.hardEdge,
  constraints: BoxConstraints(
      minWidth: double.infinity,
      minHeight: 50.0,
  ),
  decoration: BoxDecoration(
    color: Colors.white,
    image: DecorationImage(
      alignment: Alignment.bottomRight,
      image: AssetImage("assets/sample/home_banner_1.jpg"),
      fit: BoxFit.cover,
    ),
    borderRadius: BorderRadius.circular(5),
    boxShadow: [
      BoxShadow(color: Colors.black38, spreadRadius: 0, blurRadius: .5),
    ],
  ),
  transform: Matrix4.skewY(0.3),
  child: Text('容器'),
),
```

### 屬性

| class | name | desc |
| :--- | :--- | :--- |
| [Alignment?](../attribute_class/alignment.md) | alignment | 對齊 |
| [EdgeInsets?](../attribute_class/edgeinsets.md) | padding | 內間距 |
| [EdgeInsets?](../attribute_class/edgeinsets.md) | margin | 外間距 |
| [BoxDecoration?](../attribute_class/box_decoration.md) | decoration | 背景裝飾\(線框, 圓角, 背景\) |
| [BoxDecoration?](../attribute_class/box_decoration.md) | foregroundDecoration | 前景裝飾 |
| double? | width | 容器寬度 |
| double? | height | 容器高度 |
| [Matrix4?](../attribute_class/matrix4.md) | transform | 變換\(轉向, 放大縮小\) |
| [BoxConstraints?](../attribute_class/boxconstraints.md) | constraints | 容器大小限制 |
| Color? | color | 背景顏色 |
| Widget? | child | 內容 |

{% hint style="info" %}
* 如果你只需要 padding, 請使用 Padding Widget
* 如果你只需要 靠左, 請使用 Align Widget
* 如果你只需要 置中, 請使用 Center Widget
* 如果你只需要 大小外框, 請使用 SizedBox Widget
* color 不可與 decoration / color 同時使用
{% endhint %}

### 用於寬度100時可使用

```dart
width: MediaQuery.of(context).size.width,
height: MediaQuery.of(context).size.height,
```



