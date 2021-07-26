---
description: 外框線
---

# border

### 使用方式

```dart
// InputDecoration
border: OutlineInputBorder(
  borderRadius: BorderRadius.circular(0),
  border: Border.all(color: kGreyColor1, width: 1.0),
),

// BoxDecoration
border: Border.all(color: kGreyColor4, width: 0.5),
```

### Radius 圓角

```dart
// 全部
borderRadius: BorderRadius.circular(0),

// 單邊
borderRadius: BorderRadius.only(
  topLeft: Radius.circular(64)
),
```

### Border 線

```dart
// 全部
border: Border.all(color: kGreyColor1, width: 1.0)

// 單邊
border: 
    Border(
        top:    BorderSide(color: kGreyColor4, width: 1),
        bottom: BorderSide(color: kGreyColor4, width: 1),
        left:   BorderSide(color: kGreyColor4, width: 1),
        right:  BorderSide(color: kGreyColor4, width: 1),
    ),
```

{% hint style="info" %}
如果需要使用虛線外誆線, 可使用 dotted\_border 第三方套件的 DottedBorder 元件
{% endhint %}

### **可使用該屬性的元件**

* Container
  * decoration: **BoxDecoration**
    * border: **Border**
    * borderRadius: **BorderRadius**
* DropdownButtonFormField, TextFormField
  * decoration: **InputDecoration**
    * border: **OutlineInputBorder**
      * borderRadius: **BorderRadius**



