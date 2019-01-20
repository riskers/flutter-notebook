# 项目架构

```bash
| - android # android Native code
| - build # build temp code
| - ios # ios Native code
| - lib # flutter code
| - test # 测试
```

可以看出，我们大部分工作是在写 `lib` 下的 flutter 代码:

```dart
// lib/main.dart
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter',
      home: Scaffold(
        appBar: new AppBar(title: new Text('Title')),
        body: new Text('Home')
      )
    );
  }
}
```

# 一切皆 Widget

flutter 里所有的东西都是 Widget，连文字、间距这样的值也是 Widget:

```dart
Padding(
  padding: EdgeInsets.all(8.0),
  child: Text('this is text'),
)
```
