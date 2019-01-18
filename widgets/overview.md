# 项目架构

![](https://github-riskers-blog.oss-cn-qingdao.aliyuncs.com/20190106181933.png?x-oss-process=style/width)

```dart
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