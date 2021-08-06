# Builder Model \(json & map\)

### Setting

in `./build.yaml`

### How to use

1. run command

   ```text
   $ flutter packages pub run build_runner watch --delete-conflicting-outputs
   ```

2. open [json2dart-model ](https://imagine10255.github.io/json2dart-model/)website
3.  copy your json string

```dart
import 'package:json_annotation/json_annotation.dart'; // <~ this
import 'package:copy_with_extension/copy_with_extension.dart'; // <~ this

part 'state.g.dart'; // <~ this

@JsonSerializable() // <~ this
@CopyWith() // <~ add this
class System {
  System({
    this.isFetching = false,
  });

  bool? isFetching;
 
  /// JsonSerializable Build
  factory System.fromJson(Map<String, dynamic> json) => _$SystemFromJson(json); // <~ add this
  Map<String, dynamic> toJson() => _$SystemToJson(this); // <~ add this
}
```

{% hint style="info" %}
if you need use one, run commend

```bash
# 更新
$ flutter packages pub run build_runner build

# 刪除重建
$ flutter packages pub run build_runner build --delete-conflicting-outputs
```
{% endhint %}

## 調整IDEA做目錄GROUP

![](../.gitbook/assets/cleanshot-2021-08-06-at-14.42.20.jpg)



![](../.gitbook/assets/cleanshot-2021-08-06-at-14.45.14.jpg)

![](../.gitbook/assets/cleanshot-2021-08-06-at-14.44.32.jpg)

