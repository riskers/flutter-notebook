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