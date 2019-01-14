# 路由

路由是什么不用解释，几乎所有前端框架都有自己的路由体系，无非是基于 [history](https://developer.mozilla.org/en-US/docs/Web/API/Window/history) 或 [hashchange](https://developer.mozilla.org/en-US/docs/Web/Events/hashchange) 实现的。

flutter 中的路由就很简单，是原生实现的:

```dart
// push 进入路由
Navigator.push(
  context,
  MaterialPageRoute(builder: (_) => SecondScreen())
);

// pop 退出路由
Navigator.pop(context);
```

[完整代码](https://gist.github.com/riskers/4f1b9a7989b171376f725d8b75a62f46/raw/bcbca5c6e1fccfd64ee34084b7d21da06724fe32/push.dart)

另外，还有一种命名路由的方式:

```dart
// init:
return MaterialApp(
  initialRoute: '/',
  routes: {
    '/': (_) => FirstScreen(),
    '/about': (_) => SecondScreen(),
  },
);

// 进入 about 页面
Navigator.pushNamed(context, '/about');
```

[完整代码](https://gist.github.com/riskers/4f1b9a7989b171376f725d8b75a62f46/raw/bcbca5c6e1fccfd64ee34084b7d21da06724fe32/pushNamed.dart)
