# 自定义 Widget

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

## Sta

-----

[function_widget]:https://gist.githubusercontent.com/riskers/fb174083be0064aaa1c232e468ee8ed9/raw/7e1cfd2267267fa1aec5359a6517116985f8318e/function_widget.dart