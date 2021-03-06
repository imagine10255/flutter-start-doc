---
description: 簡化版的 Container (單純只提供 alignment 屬性的 Widget)
---

# Align, Center

### 使用方法

```dart
Align(
  alignment: widget.alignment,
  heightFactor: widget.verticalAnimation ? _animation.value : 1.0,
  widthFactor: widget.horizontalAnimation ? _animation.value : 1.0,
  alignment: Alignment.centerRight,
  child: Container(),
)
```

###  屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| \*[AlignmentGeometry](../attribute-class/alignment-geometry.md) | alignment | 對齊方式 |  |
| double | widthFactor | 等比縮放 |  |
| double | heightFactor | 等比縮放 |  |
| Widget | child | 內容 |  |

###  Center

Align 的簡化, 直接給你上下左右置中

```text
Center(
   child: Container(),
)
```

### 屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| Widget | child | 內容 |  |

