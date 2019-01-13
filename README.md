### Flutter 的优势

* 热加载(hot reload)是 dev 支持的 ：UI 开发提速（不用 build）https://www.infoq.cn/article/why-flutter-uses-dart

  > 注意不是热修复或热更新，目前 Flutter 不支持: https://github.com/flutter/flutter/issues/14330

* Google 下一代操作系统支持
* 比 RN 等 JS 方案快（理论上）

### for FE

针对前端来说，布局 Widget 类比 CSS，StatefulWidget 和 StatelessWidget 类比 React 组件，pub 类比 npm。

大致分为:

* widget
  * stateless
  * stateful
  * layout
  * route
  * ...
* theme
* interactivity
  * TextField
  * 手势
  * ...
* deps
  * pub
  * plugins
  * file (assets: font / image)

### for Native

对于 Native 开发者，主要工作应是:

* 开发 plugin
* 打包
* 协同
* ...


整体来说，UI 部分为前端来做，应用的是自己熟悉的思想，不过是换了框架和语言。而 App 的底层功能调用为 Native 开发 plugin 来让前端来用。

