# StatefulWidget

保存状态的 widget

实现一个 stateful 的 widget，可以继承 StatefulWidget 并在 createState 方法中返回一个 State。

```dart
// StatefulWidget 基本结构
class HelloRect extends StatefulWidget {
  HelloRect({
    this.text
  });

  final String text;

  @override
  createState() => _HelloRectState(); // 用 createState 创建一个 state 对象
}
```

State 对象存储了 WidgetState 信息并且可以在对象的声明周期中发生改变。

```dart
class _HelloRectState extends State <HelloRect> {
  var color = Colors.purple;

  @override
  Widget build(BuildContext context) {
    return Container(
      child: Text(widget.text),
      color: color,
    );
  }
}
```


[Code](https://gist.githubusercontent.com/riskers/fb174083be0064aaa1c232e468ee8ed9/raw/b44ba9870e151adaa0fac383f6ed9d5dd25b8cb0/stateful_widget.dart)