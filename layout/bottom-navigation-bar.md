# BottomNavigationBar

### 使用方法

```dart
BottomNavigationBar(
  currentIndex: currentIndex,
  onTap: onTabHandler,
  type: BottomNavigationBarType.fixed,
  selectedFontSize: 12,
  unselectedFontSize: 12,
  selectedItemColor: kPrimaryColor,
  unselectedItemColor: kGreyColor2,
  showUnselectedLabels: true,
  items: <BottomNavigationBarItem>[
    BottomNavigationBarItem(icon: Icon(IconFont.gamepad_line, size: 40), label: '遊戲'),
    BottomNavigationBarItem(icon: Icon(IconFont.bullhorn, size: 40), label: '活動'),
    BottomNavigationBarItem(icon: Icon(IconFont.ticket_alt, size: 40), label: '優惠卷'),
    BottomNavigationBarItem(icon: Icon(IconFont.book_star, size: 40), label: '贊助'),
    BottomNavigationBarItem(icon: Icon(IconFont.repeat_24_alt, size: 40), label: '客服'),
  ],
),
```

### 進階用法

配合 PageControl, [PageView](../grid/pageview.md) 做 animateToPage 來達成 帶左右移動的切換效果  
CustomBottomNavigationBar = BottomNavigationBar

```dart
class HomeGroupScreen extends StatefulWidget {
  HomeGroupScreen({Key? key}) : super(key: key);

  @override
  _HomeGroupScreenState createState() => _HomeGroupScreenState();
}

class _HomeGroupScreenState extends State<HomeGroupScreen>
    with SingleTickerProviderStateMixin {
  int _currentPageIndex = 0;
  PageController _myPage = PageController(initialPage: 0);


  @override
  void initState() {
    super.initState();
    _myPage.addListener(() {});
  }

  void _handlePageViewItemSelect(int pageIndex) {
    _myPage.animateToPage(pageIndex,
        duration: Duration(milliseconds: 300), curve: Curves.ease);
  }

  void _handleTabButtonHandler(int pageIndex) {
    setState(() {
      _currentPageIndex = pageIndex;
    });
  }


  @override
  Widget build(BuildContext context) {
    return Scaffold(
        appBar: HomeAppBar(),
        endDrawer: CustomDrawer(),
        bottomNavigationBar: CustomBottomNavigationBar(
            currentIndex: _currentPageIndex, onTap: _handlePageViewItemSelect),
        body: PageView(
          controller: _myPage,
          onPageChanged: _handleTabButtonHandler,
          children: <Widget>[
            HomeScreen(),
            PromotionScreen(),
          ],
        )
      // body: pages[_currentIndex],
    );
  }
}
```

![&#x6548;&#x679C;&#x793A;&#x610F;](../.gitbook/assets/cleanshot-2021-07-28-at-18.54.41.gif)

### 參考連結

{% embed url="https://www.programmersought.com/article/69354797891/" %}



