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
| [Alignment](https://imagine10255.gitbook.io/fluuter_start_doc/attribute_class/alignment) | alignment | 對齊 |
| [EdgeInsets](https://imagine10255.gitbook.io/fluuter_start_doc/attribute_class/edgeinsets) | padding | 內間距 |
| [EdgeInsets](https://imagine10255.gitbook.io/fluuter_start_doc/attribute_class/edgeinsets) | margin | 外間距 |
| [BoxDecoration](https://imagine10255.gitbook.io/fluuter_start_doc/attribute_class/box_decoration) | decoration | 背景裝飾\(線框, 圓角, 背景\) |
| [BoxDecoration](https://imagine10255.gitbook.io/fluuter_start_doc/attribute_class/box_decoration) | foregroundDecoration | 前景裝飾 |
| double | width | 容器寬度 |
| double | height | 容器高度 |
| Matrix4 | transform | 變換\(轉向, 放大縮小\) |
| BoxConstraints | constraints | 容器大小限制 |
| Widget | child | 內容 |

{% hint style="info" %}
如果你只需要 padding, 請使用 Padding widget  
如果你只需要 靠左, 請使用 Align widget  
如果你只需要 置中, 請使用 Center widget
{% endhint %}



