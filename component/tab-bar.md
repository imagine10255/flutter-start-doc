# TabBar

## DefaultTabController

### 使用方法

```dart
import 'package:flutter/material.dart';

/// 登入
class LoginScreen extends StatefulWidget {
  LoginScreen({Key? key}) : super(key: key);

  @override
  _LoginScreenState createState() => _LoginScreenState();
}


class _LoginScreenState extends State<LoginScreen> with SingleTickerProviderStateMixin {
    
  static const List<Tab> myTabs = <Tab>[
      Tab(text: '帳號登入'),
      Tab(text: '手機登入'),
    ];
    
    
  @override
  void initState() {
    super.initState();
    _tabController = TabController(vsync: this, length: myTabs.length);
  }

  @override
  void dispose() {
    _tabController.dispose();
    super.dispose();
  }
  
  
  /// 頁籤
  Widget _buildTabContent(BuildContext context) {
    return DefaultTabController(
      length: 2,
      initialIndex: 0,
      child: Column(
        crossAxisAlignment: CrossAxisAlignment.stretch,
        children: <Widget>[
          Container(
            padding: EdgeInsets.only(left: 20, right: 20),
            child: TabBar(
              controller: _tabController,
              labelColor: Color.fromRGBO(0, 163, 224, 1),
              unselectedLabelColor: Color.fromRGBO(141, 141, 141, 1),
              tabs: myTabs,
            ),
          ),
          Container(
            padding: EdgeInsets.only(top: 32),
            height: 600,
            decoration: BoxDecoration(
              border: Border(
                top: BorderSide(color: Colors.grey, width: 0.5)
              )
            ),
            child:
              TabBarView(
                controller: _tabController, 
                children: <Widget>[
                  Text('帳號登入內容'),
                  Textt('手機登入內容'),
                ],
              )
            ),
          ]
        )
      );
  }
        
        
}
```

{% hint style="info" %}
TabBarView 的 children 根據 TabBar 的 tabs 對應位置順序
{% endhint %}

