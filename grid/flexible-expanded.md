---
description: 占位分配
---

# Flexible, Expanded

## Flexible

### 使用方法

```dart
Flexible(
  fit: FlexFit.tight,
  child: Text('剩下的我全都要'),
);
```

### 屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| FlexFit | fit | 分配 | FlexFit.loose |
| Widget | child | 內容 |  |

* fit
  * FlexFit.loose
  * FlexFit.tight 等同於使用 Expanded flex = 1

## Expanded

### 使用方法

```dart
Expanded(
  flex: 1,
  child: Text('剩下的我全都要'),
)
```

###  屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| int | flex | 分配 | 1 |
| Widget | child | 內容 |  |



