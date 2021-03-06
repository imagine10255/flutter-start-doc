---
description: 浮動的 Widget
---

# Stack, Positioned

放在 Stack Children 中的每個 Widget 都是浮動, 越下面的層級越高

### 使用方法

```dart
Stack(
  clipBehavior: Clip.none,
  children: [
    Text('Stack!'),
    Positioned(
      bottom: 0,
      right: 10,
      child: Text('層級 zIndex-0'),
    ),
    Positioned(
      bottom: 0,
      right: 15,
      child: Text('層級 zIndex-1'),
    ),
  ],
);
```

### 屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| [AlignmentGeometry](../attribute-class/alignment-geometry.md) | alignment | 對齊方式 |  |
| [TextDirection](../attribute-class/text-direction.md) | textDirection | 對齊方向 |  |
| [StackFit](../attribute-class/stack-fit.md) | fit |  |  |
| [Clip](../attribute-class/clip.md) | clipBehavior | 類似Overflow |  |
| List&lt;Widget&gt; | children | 內容 |  |



