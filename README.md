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

