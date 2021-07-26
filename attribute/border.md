---
description: 外框線
---

# border

### 使用方式

```dart
border: OutlineInputBorder(
  borderRadius: BorderRadius.circular(0),
  border: Border.all(color: kGreyColor1, width: 1.0),
),
```

### Child Border Attribute

```dart
// 全部設定
border: Border.all(color: kGreyColor1, width: 1.0)

// 設定單邊
border: 
    Border(
        top:    BorderSide(color: kGreyColor4, width: 1),
        bottom: BorderSide(color: kGreyColor4, width: 1),
        left:   BorderSide(color: kGreyColor4, width: 1),
        right:  BorderSide(color: kGreyColor4, width: 1),
    ),
```

### **可使用該屬性的元件**

* Container
  * decoration
* TextFormField
  * decoration



