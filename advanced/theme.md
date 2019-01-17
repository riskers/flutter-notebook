TODO...

<!-- > android 和 ios 平台的差异性 -> 判断平台使用 widget
>
> 切换主题 -> Theme

# theme

```dart
import 'package:flutter/material.dart';
import 'package:flutter/cupertino.dart';

Theme.of(context).platform == TargetPlatform.iOS ?
  CupertinoSwitch(
    value: true,
    onChanged: (bool toggled) {},
  ) :
  Switch(
    value: true,
    onChanged: (bool toggled) {},
  )
```
 -->
