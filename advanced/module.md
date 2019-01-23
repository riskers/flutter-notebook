# 模块管理

flutter 中模块有以下类型:

* Application: 一个完整的应用
* Plugin: 与 iOS 或者 Android 通信的接口
* Package: flutter Widget

他们本质上都是 dart 语言包，可以发布在 pub 上，可以参见之前写过的 [给前端看的 dart 包管理与发布](https://github.com/riskers/blog/issues/46)。

上文讲了 dart 的发包，现在说下 dart 中模块的引用和使用(引用本地文件):

```dart
import './some_widget/some_widget.dart';
```

这是相对路径，但也是 dart 不推荐的方法，实际上，你可以这么引用(确保 `pubspec.yaml` 中 `name` 字段是 `flutter_demo`):

```dart
import 'package:flutter_demo/some_widget/some_widget.dart';
```
