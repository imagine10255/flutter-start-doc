# MaterialApp

### 使用方法

```dart
MaterialApp(
  debugShowCheckedModeBanner: false,
  navigatorKey: NavigatorHolder.navigatorKey,
  theme: customThemeLight,
  title: 'Flutter StartKit',
  localizationsDelegates: localizationsDelegates,
  supportedLocales: supportedLocales,
  locale: currentLocale,
  initialRoute: initialRoute,
  routes: routes,
  navigatorObservers: [
    RouterObserver(),
  ],
  onUnknownRoute: onUnknownRoute,
  // builder: (BuildContext context, Widget? child) {
  //   return Stack(
  //     children: [
  //       child!,
  //     ],
  //   );
  // },
);
```

 

