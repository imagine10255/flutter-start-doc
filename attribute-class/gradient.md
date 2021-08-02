---
description: 漸層變色
---

# Gradient

## LinearGradient 線性變色

![&#x793A;&#x610F;&#x5716;](../.gitbook/assets/cleanshot-2021-08-02-at-10.27.34.jpg)

```text
LinearGradient(
  begin: Alignment.topLeft,
  end: Alignment.bottomRight,
  stops: [
    .5,
    .5
  ],
  colors: [
    Color.fromRGBO(246, 246, 250, 1),
    Color.fromRGBO(236, 236, 246, 1),
    // Colors.transparent,
  ],
)
```

### 屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| [AlignmentGeometry](alignment-geometry.md) | begin | 內間距 |  |
| [AlignmentGeometry](alignment-geometry.md) | end | 內容 |  |
| List&lt;double&gt; | stops |  |  |
| List&lt;Color&gt; | colors | 顏色 |  |
| TileMode | tileMode |  |  |
| [GradientTransform](gradienttransform.md) | transform |  |  |

