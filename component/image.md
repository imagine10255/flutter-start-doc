---
description: 圖片
---

# Image

### 使用方法

本地資源

```dart
// jpg, png
Image.asset('images/image.png')

// svg
SvgPicture.asset(
    'assets/images/logo.svg',
    semanticsLabel: 'My Logo', 
    width: 80
),
```

 網路資源

```dart
// jpg, png
Image.network('images/image.png')

// svg
SvgPicture.network(
    'assets/images/logo.svg',
    semanticsLabel: 'My Logo', 
    width: 80
),
```

{% hint style="info" %}
SVG 為第三方套件 flutter\_svg  
注意這邊回傳的是 Widget, 不是 [ImageProvider](../attribute-class/image-provider.md)
{% endhint %}

