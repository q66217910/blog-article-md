# blog-article-md
md格式博客文章

下面需要两个文件夹`static`和`_posts`
`_posts`文件夹存储md格式文章，文章要求，md格式文章开头必须是如下格式

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
rId：在数据库中文章的unique字段，相同rId的文章会被识别为同一篇


`static`文件夹存储图片/附件等在`_posts`文件中引用的附件或图片
