+++
title = 'Hugo指南'
date = 2024-06-11T12:06:50+08:00
draft = false
+++

## 常用命令
1. 添加post
```shell
hugo new posts/my-new-post.md
```

## 问题

1.  papermod在hugo server --destination和hugo server显示的主页不一样 检查 Front Matter的draft属性

## 知识点

1. 在 Hugo 中，文章文件的前端信息（Front Matter）用于定义元数据，如标题、日期、标签等。前端信息可以使用三种格式：YAML、TOML 和 JSON。不同格式使用的分隔符不同：
> - YAML：使用 `---` 作为分隔符。
> - TOML：使用 `+++` 作为分隔符。
> - JSON：使用 `{` 和 `}` 作为分隔符。
 
2. hugo直接嵌入在`posts`文件夹的图片，编译后会产生路径问题，需要在`config.toml`中配置`assetDir`属性，指定图片路径

3. 如何显示图片
> https://www.yuweihung.com/posts/2021/hugo-blog-picture/
缺点：都叫index.md，不好区分
