# Decoration

## BoxDecoration

BoxDecoration是Decoration的一個實現類，BoxDecoration提供了背景顏色、邊框、陰影、圓角、顏色漸變、形狀等等裝飾能力

### 使用方法

```dart
decoration: BoxDecoration(
  color: Colors.white,
  image: DecorationImage(
    alignment: Alignment.bottomRight,
    image: AssetImage("assets/sample/home_banner_1.jpg"),
    fit: BoxFit.cover,
  ),
  borderRadius: BorderRadius.circular(5),
  boxShadow: [
    BoxShadow(color: Colors.black38, spreadRadius: 0, blurRadius: .5),
  ],
),
```

### 屬性

| Class | Name | Desc | Default |
| :--- | :--- | :--- | :--- |
| Color | color | 背景顏色 |  |
| [DecorationImage](decoration-image.md) | image | 背景圖片，會在背景顏色上面 |  |
| [BoxBorder](box-border.md) | border | 邊框，會畫在背景顏色上 |  |
| [BorderRadiusGeometry](border-radius-geometry.md) | borderRadius | 邊框圓角 |  |
| List&lt;[BoxShadow](box-shadow.md)&gt; | boxShadow | 背景陰影 |  |
| [Gradient](gradient.md) | gradient | 漸變顏色 |  |
| [BlendMode](blend-mode.md) | backgroundBlendMode | 背景混合模式 |  |
| [BoxShape](box-shape.md) | shape | 形狀 | BoxShape.rectangle |

{% hint style="info" %}
如果在 Container 有設定 color 的話, 加上decoration屬性則必須將 color 屬性 移動到 decoration 中
{% endhint %}

### 主題設定

```dart
ThemeData customThemeLight = ThemeData.from(
    colorScheme: ColorScheme.light().copyWith(
)).copyWith(
  platform: TargetPlatform.iOS,
  inputDecorationTheme: InputDecorationTheme().copyWith(
    helperStyle: TextStyle(color: CustomThemeData.gray0),
  ),
);
```

###  參考連結

{% embed url="https://www.jianshu.com/p/8e187ee57743" %}

{% embed url="https://blog.csdn.net/chenlove1/article/details/83627831" %}





