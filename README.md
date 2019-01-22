[进度](https://github.com/riskers/flutter-notebook/issues/1)

[Flutter](https://flutter.io/) 是 Google 出品的一款跨终端开发的框架，为什么要选择它？

* 热加载(hot reload)是 dev 支持的 ：UI 开发提速（不用 build）https://www.infoq.cn/article/why-flutter-uses-dart

  > 注意不是热修复或热更新，目前 Flutter 不支持: https://github.com/flutter/flutter/issues/14330

* 理论上比 RN 等基于 JavaScript 的方案快
* Google 下一代操作系统支持

针对前端来说，布局 Widget 类比 CSS，StatefulWidget 和 StatelessWidget 类比 React 组件，pub 类比 npm。

对于 Native 开发者，主要工作应是:开发 plugin、打包、协同等等。

整体来说，UI 部分为前端来做，应用的是自己熟悉的思想，不过是换了框架和语言。而 App 的底层功能调用为 Native 开发 plugin 来让前端来用。

## 目录

详见 [SUMMARY](./SUMMARY.md)

其中，前三章是对前端写的，后面则是对原生开发写的。

## 为什么要写这本书

自己也是刚上手，觉得很多概念很熟悉，入门成本不算高，就开始自己写这本书，也算是对 flutter 一个总结。

## 本书适合这样的前端

* 熟练 CSS，尤其是各种布局方式，比如 position、flex
* 有 TypeScript 或其他静态语言基础
* 操练过 React / Vue 这一类框架
* 想耍耍 Native 开发却不知如何开始，就从 plugin 开始

## 能够学到

* flutter 组件类型和常用组件介绍
* flutter 数据管理、主题管理、依赖管理等

