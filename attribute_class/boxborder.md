# BoxBorder

## Border

### 使用方式

```dart
// 全部
Border.all(
  color: kGreyColor1, 
  width: 1.0
)


// 單邊
Border(
  top: BorderSide(
    color: kGreyColor4, 
    width: 1,
  ),
  bottom: BorderSide(
    color: kGreyColor4, 
    width: 1,
  ),
  left: BorderSide(
    color: kGreyColor4, 
    width: 1,
  ),
  right: BorderSide(
    color: kGreyColor4, 
    width: 1,
  ),
)
```

### 屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| [BorderSide](borderside.md) | top | 邊框方向 | BorderSide.none |
| [BorderSide](borderside.md) | bottom | 邊框方向 | BorderSide.none |
| [BorderSide](borderside.md) | left | 邊框方向 | BorderSide.none |
| [BorderSide](borderside.md) | right | 邊框方向 | BorderSide.none |

## BorderDirectional

### 使用方式

```text
BorderDirectional(
  top: BorderSide.none,
  start: BorderSide.none,
  end: BorderSide.none,
  bottom: BorderSide.none,
)
```



### 參考連結

[https://api.flutter.dev/flutter/painting/Border-class.html](https://api.flutter.dev/flutter/painting/Border-class.html)

