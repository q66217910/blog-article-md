# blog-article-md
md格式博客文章

## 文件夹格式规则
下面需要两个文件夹`static`和`_posts`
`_posts`文件夹存储md格式文章
`static`文件夹存储图片/附件等在`_posts`文件中引用的附件或图片

## 文章格式规则

文章文件名没有做要求，但为了方便管理，按一定规则存放比较好，如：年-月-日_英文名称.md

文章要求，md格式文章开头必须是如下格式

```
---
title: 博客标题
date: 2017-03-19 12:08:42
tags: maven
permalink: maven-filter
keywords: maven, Invalid keystore format, jks
rId: MB-17031901
---
```
上述格式中各行的解释

title：文章标题 

date：希望网站显示的文章发布时间 

tags：文章标签（只能有一个） 

keywords：文章关键字，可以有多个，以英文逗号分隔 

permalink：文章在网站上链接地址名（实际上网站上会以 `yyyy-MM-dd + - + permalink` 作为文章链接地址） 

rId：在数据库中文章的unique字段，相同rId的文章会被识别为同一篇。为了方便管理，建议使用 `年月日 + 该日第几篇` 格式较为合适，同样，附件文件夹中附件名也建议使用 `rId + 该篇第几个附件` 来命名

可选属性

originId：该参数是针对文章改变了rId的场景提供的，该参数表示文章的原先使用的rId，方便后台将文章从旧的rId变更为新的rId
