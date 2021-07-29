# Builder Model \(json & map\)

### Setting

in `./build.yaml`

### How to use

1. run command

   ```text
   $ flutter packages pub run build_runner watch --delete-conflicting-outputs
   ```

2. open [quicktype](https://app.quicktype.io/) website
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
$ flutter packages pub run build_runner build
```
{% endhint %}

![](../.gitbook/assets/image%20%282%29.png)

