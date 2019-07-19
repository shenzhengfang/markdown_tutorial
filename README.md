# markdown_tutorial

- [Markdown 目录树](#Markdown-目录树)
- [页内跳转](#页内跳转)
- [自定义锚](#自定义锚)
- [markdown 学习资源](#markdown-学习资源)

### Markdown 目录树

想要给文档生成目录树，只需要在文档中增加 `[TOC]` ，目录树就会根据文档中的 `h1~h6` 标题自动生成了。

### 页内跳转

Markdown会自动给每一个h1~h6标题生成一个锚，其id就是标题内容。目录树中的每一项都是一个跳转链接，点击后就会跳转到其对应的锚点（即标题所在位置）。你可以点击本文档开始处的目录树尝试一下。

如果需要在目录树之外还要增加跳转到某个标题的链接，则有两种办法可以做到： 
1. 使用Markdown的语法来增加跳转链接：`“[名称](#id)”`。 
2. 使用HTML语法来增加跳转链接：`“<a href=”#id”>名称`

>注意：id里不能包含符号，如果有空格用 - 代替
>
>比如：
>
>1、test test = [1、test test](#1test-test)

其中的“名称”可以随便填写，“id”需要填写跳转到的标题的内容。

例如如果想要增加一个到本文档“markdown_tutorial”标题的跳转链接，则需要这么写：

`[markdown_tutorial](#markdown_tutorial)` = [markdown_tutorial](#markdown_tutorial)

或者

`<a href=”#markdown_tutorial”>markdown_tutorial` = <a href="#markdown_tutorial">markdown_tutorial

### 自定义锚

假设我们想跳转到文档中的一个不是标题的位置（比如一张图表），则需要在该位置自定义一个锚。

我们使用HTML语法来定义一个锚。可选的HTML标签很多，比如`<span>、<a>`等等。本文使用`<span>`示例。

假设文档中有一个作息时间表，在文档的其他地方需要增加跳转到此表位置的链接，那么我们可以在此表的附近增加一行：

锚点：`<span id="bryanshen">bryanshen</span>` = <span id="bryanshen">bryanshen</span>
>注：id 为必填项；“名称”可以随便填写，也可以不填。另外，可以给 `span` 增加其他属性，比如颜色等等。

跳转超链接：
* `[bryanshen](#bryanshen)` = [bryanshen](#bryanshen)
* `<a href="#bryanshen">bryanshen` = <a href="#bryanshen">bryanshen

### markdown 学习资源
* [Learning-Markdown（Markdown 入门参考）](http://xianbai.me/learn-md/article/syntax/images.html)
