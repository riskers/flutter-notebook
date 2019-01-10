# WidgetStateless

## 函数 Widget

写过 React 的人都知道纯函数组件，flutter 类比过来可以是这样:

```dart
Widget helloRect() {
  return Container(
    color: Colors.purple,
    width: 200,
    height: 200,
    margin: EdgeInsets.all(16),
    child: Center(child: Text('Hi')),
  );
}
```

[Code][function_widget]

<image src="./assets/function_widget.png" width="300" />

## StatelessWidget

但是 Flutter 中最常用的是 StatelessWidget:

```dart
class HelloRect extends StatelessWidget {
  final String text;

  HelloRect({this.text});

  @override
  Widget build(BuildContext context) {
    return Container(
      color: Colors.purple,
      width: 200,
      height: 200,
      margin: EdgeInsets.all(16),
      child: Center(child: Text(text)),
    );
  }
}
```

[Code][stateless_widget]

<image src="./assets/stateless_widget.png" width="300" />

## 从 dart 语法来看 Widget 参数

上面的语法对于 dart 不熟悉的人可能会看不懂，这其实是 dart 的语法糖，不用的话就是这样:

```dart
// 不使用语法糖
class HelloRect extends StatelessWidget {
  final String text;

  // HelloRect({this.text});  // 在构造函数中可以直接将 this 替换
  HelloRect({String text}) { // text 是 String 类型的可选参数
    this.text = text;
  }

  @override
  Widget build(BuildContext context) {
    return Container(
      color: Colors.purple,
      width: 200,
      height: 200,
      margin: EdgeInsets.all(16),
      // child: Center(child: Text(text)),  // dart 中 this 是可省略的
      child: Center(child: Text(this.text)),
    );
  }
}
```

这一段看懂之后就运行下面的代码，再看效果 :

[Code][stateless_widget_multi_params]

<image src="./assets/stateless_widget_multi_params.png" width="300" />

-----

[function_widget]:https://gist.githubusercontent.com/riskers/fb174083be0064aaa1c232e468ee8ed9/raw/7e1cfd2267267fa1aec5359a6517116985f8318e/function_widget.dart
[stateless_widget]:https://gist.githubusercontent.com/riskers/fb174083be0064aaa1c232e468ee8ed9/raw/f5cb58dea28d71a9a4b4fca979e3f14697462791/stateless_widget.dart
[stateless_widget_multi_params]:https://gist.githubusercontent.com/riskers/fb174083be0064aaa1c232e468ee8ed9/raw/ced8bda7d485ebc5cb6f2ab0e2a8fa35804f1223/stateless_widget_multi_params.dart