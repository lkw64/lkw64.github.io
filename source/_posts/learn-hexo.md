---
title: learn hexo
date: 2019-05-19 20:34:45
tags:
---
## 标签插件(Tag Plugings)
标签插件和Front-matter中的标签不同，它们是用于在文章中快速插入特定内容的插件。
### 引用块
在文章中插入引言，可包含作者、来源和标题。

**别号：**quote
```
{% blockquote [author[, source]] [link] [source_link_title] %}
content
{% endblockquote %}
```
<!--more-->
#### 样例

**没有提供参数，则只输出普通的blockquote**
```
{% blockquote %}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque hendrerit lacus ut purus iaculis feugiat. Sed nec tempor elit, quis aliquam neque. Curabitur sed diam eget dolor fermentum semper at eu lorem.
{% endblockquote %}
```
>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque hendrerit lacus ut purus iaculis feugiat. Sed nec tempor elit, quis aliquam neque. Curabitur sed diam eget dolor fermentum semper at eu lorem.

{% blockquote [author[, source]] [link] [source_link_title] %}
Do not seek happiness for yourself. Seek happiness for all. Through kindness. Through mercy.
{% endblockquote %}
{% codeblock %}
alert('Hello World!') <button>
[comment]:下面的渲染结果到底是怎么来的？从上面的渲染结果来看，应该不是大括号造成的。为什么会有这么个块结构呢？要怎么才能让继续内容脱离这么块结构？而且，在浏览器中，代码块显示了，而且notepad++隐藏的内容显示了，但为什么后面的内容却不显示呢？去掉尖括号后，块结构消失了。应该是尖括号问题？空尖括号不会出现块，尖括号中有英文字符出现方框包含的块。
{% endcodeblock %}  

![](../images/zhwdm.png)
