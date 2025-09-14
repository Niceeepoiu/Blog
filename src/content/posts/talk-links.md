---
title: 关于博客“正常”的链接
published: 2025-09-12
description: '讨论博客里那些奇奇怪怪的链接'
image: ''
tags: ["链接","博客"]
category: '电子杂谈'
draft: false 
---

在写这篇文章<https://niceeepoiu.netlify.app/posts/tools-1/> 时 ，发现链接似乎不止停留在单纯的普通段落。

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.0.1/css/all.min.css">

## 首先你要这样做

```markdown
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.0.1/css/all.min.css">
```

使用Font Awesome的在线图标dll是~~整活~~实验的关键！

### 为什么能在Markdown里使用HTML代码？

~~因为我足够帅气逼人~~

具体来说，博客网页里的Markdown文章不能直接显示，需要先读取YAML元数据获取文章信息，然后将文章转换为HTML，而HTML段落会被转换为`<p>`标签，应该显示为段落吧？蛋柿，`<p>`标签里也可以插入HTML代码，比如这样：

```html
<p><mark>这应该不是段落</mark></p>
```

<p><mark>这应该不是段落</mark></p>

所以，理论来说，将Markdown转换为HTML的渲染器应该都支持HTML代码，而HTML里又支持CSS和Javascript代码，所以CSS和Javascript代码也是同理。

## 然后就可以开始~~整活~~实验了

这是图标链接

**Python：** [<i class="fa-brands fa-python"></i>](https://www.python.org/)

你还可以这样

[<mark><i class="fa-brands fa-python"></i></mark>](https://www.python.org/)

隐身链接，不会有人找不到吧？

[     ](https://www.python.org/)
