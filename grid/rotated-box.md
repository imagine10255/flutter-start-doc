---
description: 轉向 Widget
---

# RotatedBox

### 使用方法

```text
RotatedBox(
  quarterTurns: isExpanded ? 3 : 1,
  child: Icon(IconFont.chevron_right_thin, color: kGreenColor, size: 20),
)
```

###  屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| \*int | quarterTurns | 轉向方向 |  |
| Widget | child | 內容 |  |

* quarterTurns: 
  * 0=右
  * 1=下
  * 2=左 
  * 3=上

