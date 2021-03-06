---
description: 變形
---

# Transform

### 使用方法

```dart
Transform(
  alignment: Alignment.topRight,
  transform: Matrix4.skewY(0.3)..rotateZ(-math.pi / 12.0),
  ild: Container(
    padding: EdgeInsets.all(8.0),
    color: Color(0xFFE8581C),
    child: Text('Apartment for rent!'),
  ),
),
```

##  Transform.rotate

### 使用方法

```dart
import 'dart:math' as math;

Transform.rotate(
  angle: math.pi/2,
  child: Icon(IconFont.chevron_right_thin, color: kGreyColor2, size: 20),
)
```

### 屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| double | angle | 轉向 |  |
| Widget | child | 內容 |  |

* angle:
  *  math.pi/2 = 下
  * 0 = 右 

## Transform.translate

### 使用方法

```dart
Transform.translate(
  offset: Offset(0.0, 15.0),
  child: Container(
    padding: EdgeInsets.all(8.0),
    color: Color(0xFF7F7F7F),
    child: Text('Quarter'),
  ),
)
```

### 屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| [Offset](../attribute-class/offset.md) | offset | 偏移位置 |  |
| Widget | child | 內容 |  |

## Transform.scale

### 使用方法

```dart
Transform.scale(
  scale: 0.5,
  child: Container(
    padding: EdgeInsets.all(8.0),
    color: Color(0xFFE8581C),
    child: Text('Bad Idea Bears'),
  ),
)
```

### 屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| double | scale | 偏移位置 |  |
| Widget | child | 內容 |  |

