---
description: 簡化版的 Container (單純只提供 裁切 屬性的 Widget)
---

# ClipRRect

### 使用方法

```dart
ClipRRect(
  borderRadius: BorderRadius.only(
    topLeft: Radius.circular(15.0),
    topRight: Radius.circular(15.0),
  ),
)
```

### 屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| [BorderRadius](../attribute-class/border-radius-geometry.md#borderradius) | borderRadius | 圓角 | BorderRadius.zero |
| CustomClipper&lt;RRect&gt; | clipper |  |  |
| [Clip](../attribute-class/clip.md) | clipBehavior |  |  |
| Widget | child | 內容 |  |

###  參考連結

{% embed url="https://segmentfault.com/a/1190000015149101" %}



