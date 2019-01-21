## Text

## Image

```dart
new Image.network(
    'https://ws1.sinaimg.cn/large/8e495e65ly1fyx06fa2d9j208s07agm5.jpg',
    fit: BoxFit.cover,
    repeat: ImageRepeat.repeatX,
),
```

| Flutter | CSS |
| :-- | :-- |
| BoxFit.cover | background-size: cover |
| BoxFit.contain | background-size: contain |
| ImageRepeat.repeatX | background-repeat: repeat-x |
| ImageRepeat.repeatY | background-repeat: repeat-y |

## Row

* 不灵活布局:
* 灵活布局 `Expanded`: 平均分配，一行充满

第三个 button 是自由伸缩的，前两个是 Expanded 的。

![](https://github-riskers-blog.oss-cn-qingdao.aliyuncs.com/20190106204815.png?x-oss-process=style/width)

[Code](https://gist.github.com/riskers/ee71c1754117981bf7358359b390ff4e#file-row-dart)

## Column

![](https://github-riskers-blog.oss-cn-qingdao.aliyuncs.com/20190106210938.png?x-oss-process=style/width)

[Code](https://gist.github.com/riskers/ee71c1754117981bf7358359b390ff4e#file-column-dart)

## Stack

![](https://github-riskers-blog.oss-cn-qingdao.aliyuncs.com/20190106213438.png?x-oss-process=style/width)

[Code](https://gist.github.com/riskers/ee71c1754117981bf7358359b390ff4e#file-stack-dart)

