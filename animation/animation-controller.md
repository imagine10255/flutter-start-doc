---
description: 動畫控制器
---

# AnimationController



{% hint style="info" %}
forward 正向  
reverse 反向  
repeat 重複動畫  
如果在 ..repeat\(reverse: true\) 則會正向動畫後 進行反向動畫, 再循環
{% endhint %}

```dart
class RefreshAmountButton extends StatefulWidget {
  @override
  _RefreshAmountButtonState createState() => _RefreshAmountButtonState();
}

class _RefreshAmountButtonState extends State<RefreshAmountButton> with TickerProviderStateMixin {

  late final AnimationController _controller;
  late final Animation<double> _animation;


@override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  @override
  void initState() {
    super.initState();

    _controller = AnimationController(
        duration: Duration(seconds: 2),
        vsync: this,
        reverseDuration: Duration(seconds: 0),
    )..repeat(reverse: false);

    _animation = CurvedAnimation(
      parent: _controller,
      curve: Curves.linear,
    );
  
  }
  
  
  
  
  @override
  Widget build(BuildContext context) {
  
      return RotationTransition(
          turns: _animation,
          child:  TextButton(
            child: Icon(IconFont.redo, color: kPrimaryColor, size: 20),
            style: TextButton.styleFrom(padding: EdgeInsets.all(4), primary: kGreyColor),
            onPressed: () => store.dispatch(FetchWalletAmountAction()),
          ),
        );
  }
}
```

