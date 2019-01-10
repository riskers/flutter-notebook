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

## 布局

针对麻烦的布局问题:

* Alt + Enter: 快捷操作 Widget

## Text

## Image

```dart
new Image.network(
    'https://ws1.sinaimg.cn/large/8e495e65ly1fyx06fa2d9j208s07agm5.jpg',
    fit: BoxFit.cover,
    repeat: ImageRepeat.repeatX,
),
```

| Flutter | CSS |
| :-- | :-- |
| BoxFit.cover | background-size: cover |
| BoxFit.contain | background-size: contain |
| ImageRepeat.repeatX | background-repeat: repeat-x |
| ImageRepeat.repeatY | background-repeat: repeat-y |

## ListView

### 静态

![](https://github-riskers-blog.oss-cn-qingdao.aliyuncs.com/20190106185106.png?x-oss-process=style/width)

[Code](https://gist.github.com/riskers/ee71c1754117981bf7358359b390ff4e#file-dynamic-listview-dart)

### 动态

![](https://github-riskers-blog.oss-cn-qingdao.aliyuncs.com/20190106192454.png?x-oss-process=style/width)

[Code](https://gist.github.com/riskers/ee71c1754117981bf7358359b390ff4e#file-static-listview-dart)


## GridView

![](https://github-riskers-blog.oss-cn-qingdao.aliyuncs.com/20190106202254.png?x-oss-process=style/width)

[Code](https://gist.github.com/riskers/ee71c1754117981bf7358359b390ff4e#file-gridview-dart)

## Row

* 不灵活布局: 
* 灵活布局 `Expanded`: 平均分配，一行充满

第三个 button 是自由伸缩的，前两个是 Expanded 的。

![](https://github-riskers-blog.oss-cn-qingdao.aliyuncs.com/20190106204815.png?x-oss-process=style/width)

[Code](https://gist.github.com/riskers/ee71c1754117981bf7358359b390ff4e#file-row-dart)

## Column

![](https://github-riskers-blog.oss-cn-qingdao.aliyuncs.com/20190106210938.png?x-oss-process=style/width)

[Code](https://gist.github.com/riskers/ee71c1754117981bf7358359b390ff4e#file-column-dart)

## Stack

![](https://github-riskers-blog.oss-cn-qingdao.aliyuncs.com/20190106213438.png?x-oss-process=style/width)

[Code](https://gist.github.com/riskers/ee71c1754117981bf7358359b390ff4e#file-stack-dart)

## navigator

[Code](https://gist.github.com/riskers/ee71c1754117981bf7358359b390ff4e#file-navigator-dart)

# Widget

## StatelessWidget

## StatefulWidget

### State

一个StatefulWidget类会对应一个State类，State表示与其对应的StatefulWidget要维护的状态