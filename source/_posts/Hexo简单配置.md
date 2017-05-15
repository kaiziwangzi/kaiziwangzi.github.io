---
title: Hexo操作记录
date: 2017-03-11 12:54:49
tags: hexo
---
# Hexo操作记录

标签： hexo

---

> * Note：仅记录使用hexo过程中的需求问题

## 首页显示"阅读全文" ##

当遇到这样的需求：`在首页不想大篇幅显示文章内容时，只想显示部分`，此时可以如下配置：
> 在`themes/next(主题名称)/_config.yml`中修改或添加`auto_excerpt`，将`enable`设置为true打开，`length`属性为需要显示的内容长度
```
# Automatically Excerpt. Not recommend.
# Please use <!-- more --> in the post to control excerpt accurately.
auto_excerpt:
  enable: true
  length: 500
```
<!--more-->
此时距离成功还有最后一步，当修改上面的`auto_excert`之后，是显示了部分内容，但是排版是有问题的，上面的注释已经说明了问题，需要在想要任何显示部分的地方加上`<!--more-->`，此时可以忽略`length`，再一次部署之后就是想要的结果。
>  <b>END</b>
