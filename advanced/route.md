```dart
Navigator.of(context).push(MaterialPageRoute<Null>(
  builder: (BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        elevation: 1.0,
        title: Text(
          name,
          style: Theme.of(context).textTheme.display1,
        ),
        centerTitle: true,
        backgroundColor: color,
      ),
      body: ConverterRoute(
        color: color,
        name: name,
        units: units,
      ),
    );
  },
));
```