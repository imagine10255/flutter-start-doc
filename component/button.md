---
description: 按鈕
---

# Button

## TextButton

一般按鈕 \(已棄用的對應按鈕為 FlatButton\)

### 使用方法

```dart
TextButton(
  child: Column(
    children: [
      SvgPicture.asset('assets/images/icon_svg/dollar_down.svg',
          width: 50),
      Text('圖片文字',
          style:
          TextStyle(fontWeight: FontWeight.w300, fontSize: 12)),
    ],
  ),
  onPressed: () => {},
)
```

## ElevatedButton

### 使用方法

點擊會有外框陰影的按鈕  \(已棄用的對應按鈕為 RaisedButton\)

```text
ElevatedButton(
  child: Text('Get Temporary Directory'),
  onPressed: () => {},
),
```

 

## OutlinedButton

### 使用方法

只有外框線的按鈕 \(已棄用的對應按鈕為 OutlineButton, 差一個d\)



### 參考連結

{% embed url="https://flutter.dev/docs/release/breaking-changes/buttons" %}



