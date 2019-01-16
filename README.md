[进度](https://github.com/riskers/flutter-notebook/issues/1)

[Flutter](https://flutter.io/) 是 Google 出品的一款跨终端开发的框架，为什么要选择它？

* 热加载(hot reload)是 dev 支持的 ：UI 开发提速（不用 build）https://www.infoq.cn/article/why-flutter-uses-dart

  > 注意不是热修复或热更新，目前 Flutter 不支持: https://github.com/flutter/flutter/issues/14330

* 理论上比 RN 等基于 JavaScript 的方案快
* Google 下一代操作系统支持

针对前端来说，布局 Widget 类比 CSS，StatefulWidget 和 StatelessWidget 类比 React 组件，pub 类比 npm。

对于 Native 开发者，主要工作应是:开发 plugin、打包、协同等等。

整体来说，UI 部分为前端来做，应用的是自己熟悉的思想，不过是换了框架和语言。而 App 的底层功能调用为 Native 开发 plugin 来让前端来用。

为什么要写这本书？

自己也是刚上手，觉得很多概念很熟悉，入门成本不算高，就开始自己写这本书，也算是对 flutter 一个总结。

## 目录

* 组件
  * [概述](./widgets/README.md)
  * [StatelessWidget](./widgets/statelesswidget.md)
  * [StatefulWidget](./widgets/statefulwidget.md)
* 进阶
  * 主题
  * [路由](./advanced/route.md)
  * 模块依赖
  * 动画
  * 状态管理
* Example
  * data-flow
* Native
  * 通信
  * plugin 开发
  * 在 Android 项目中集成
  * 在 iOS 项目中集成
* 团队协作
  * [Lint 工具](./team/lint.md)
  * [工程管理](./team/product.md)
* 其他
  * [技巧](./ending/tips.md)
  * [总结](./ending/README.md)

其中，前三章是对前端写的，后面则是对原生开发写的。
