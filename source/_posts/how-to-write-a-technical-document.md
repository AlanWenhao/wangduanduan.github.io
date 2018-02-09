---
title: 如何写好技术文档?
date: 2018-02-09 12:52:57
tags:
- 文档
---

> 本文来自于公司内部的一个分享。
> 在文档方面，对内的一些接口文档主要是用swagger来写的。虽然可以在线测试，比较方便。但是也存在着一些更新不及时，swgger文档无法导出成文件的问题。
> 在对外提供的文档方面：我主要负责做一个浏览器端的一个js sdk。文档还算可以[github地址](https://github.com/wangduanduan/wellclient)，所以想把一些写文档的心得分享给大家。

# 1. 衡量好文档的唯一标准是什么？

![](http://p3alsaatj.bkt.clouddn.com/20180209125351_QEkv8l_Screenshot.jpeg)

Martin(Bob大叔)曾在《代码整洁之道》一书打趣地说：当你的代码在做 Code Review 时，审查者要是愤怒地吼道：

```
“What the fuck is this shit?”
“Dude, What the fuck！”
```
等言辞激烈的词语时，那说明你写的代码是 Bad Code，如果审查者只是漫不经心的吐出几个

`“What the fuck?”，`


![](http://p3alsaatj.bkt.clouddn.com/20180209125409_sQvHfi_Screenshot.jpeg)


那说明你写的是 Good Code。衡量代码质量的唯一标准就`是每分钟骂出“WTF” 的频率`。

衡量文档的标准也是如此。


# 2. 好文档的特点
- `简洁`：一句话可以说完的事情，就不要分两句话来说。并不是文档越厚越好，太厚的文档大多没人看。
- `准确`: 字段类型，默认值，备注，是否必填等属性说明。
- `逻辑性`: 文档如何划分？ 利于查看。
- `demo胜千言`: 好的demo胜过各种字段说明，可以复制下来直接使用。
- `读者心`: 从读者的角度考虑, 方法尽量简洁。可以传递一个参数搞定的事情，绝对不要让用户去传两个参数。
- `及时更新`: 不更新的文档比bug更严重。
- `向后兼容`: 不要随意废弃已有的接口或者某个字段，除非你考虑到这样做的后果。
- `建立文档词汇表`：每个概念只有一个名字，不要随意起名字，名不正则言不顺。
- `格式统一`：例如时间格式。我曾见过2017-09-12 09:32:23, 或2017.09.12 09:32:23或2017.09.12 09:32:23。变量名user_name, userName。
- `使用专业词语`：不要过于口语化

# 3. 总结: 写出好文档要有以下四点
 1. `逻辑性`：便于查找
 2. `专业性`: 值得信赖，质量保证
 3. `责任心`：及时更新，准确性，向后兼容
 4. `读者心`：你了解的东西，别人可能并不清楚。从读者的角度去考虑，他们需要什么，而不是一味去强调你能提供什么。

# 4. 写文档的工具
- markdown: 方便快捷，可以导出各种格式的文件
- swagger: 功能强大，需要部署，不方便传递文件

# 5. markdown 工具推荐
- [蚂蚁笔记](https://leanote.com/) 这是我正使用的。
    - 全平台（mac windows ios）有客户端，和浏览器端
    - 笔记可以直接公布为博客
    - 支持独立域名
    - 标签很好用
    - 支持思维导图
    - 支持历史记录
- [cmd-markdown](https://www.zybuluo.com/mdeditor#411452)
- 有道云笔记

# 6. 文档之外
公司有个同事，我曾问他使用什么搜索一些技术文档，他说用百度。作为一个翻墙老司机，我惊诧的问他：你为什么不用谷歌去搜索。他说他不会翻墙。我只能呵呵一笑。

自从有一次搜索：`graph for x^8 + y^8`，我就决定不再使用百度了。你可以看一下两者的返回结果有什么不同。

**总之：`有些鸟儿是关不住的 他们的羽毛太鲜亮了`。**

![](http://p3alsaatj.bkt.clouddn.com/20180209125425_frCDAB_Screenshot.jpeg)
![](http://p3alsaatj.bkt.clouddn.com/20180209125433_KKkTLQ_Screenshot.jpeg)

  [1]: /img/bVXUY5
  [2]: /img/bVXUY8