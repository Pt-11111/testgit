## 元素和属性的选择
xml语言中：元数据（有关数据的数据）应当存储为属性，而数据本身应当存储为元素。

例如：
```
<messages>
<note id="501">
<to>Tove</to>
<from>Jani</from>
<heading>Reminder</heading>
<body>Don't forget me this weekend!</body>
</note>
<note id="502">
<to>Jani</to>
<from>Tove</from>
<heading>Re: Reminder</heading>
<body>I will not</body>
</note>
</messages>
```

其中 id是用来表示一条数据的而不是数据本身，所以用属性来表示。

## 形式良好的 XML 文档
"形式良好"的 XML 文档拥有正确的语法。

在前面的章节描述的语法规则：

XML 文档必须有一个根元素
XML元素都必须有一个关闭标签
XML 标签对大小写敏感
XML 元素必须被正确的嵌套
XML 属性值必须加引号

## XML 声明
XML 声明文件的可选部分，如果存在需要放在文档的第一行，如下所示：

<?xml version="1.0" encoding="utf-8"?>   注意结尾的"?"号

