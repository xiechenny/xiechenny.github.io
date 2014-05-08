---
layout: post
title: "Octopress写多彩的博文"
date: 2014-05-07 16:22:17 +0800
comments: true
categories: "octopress"
---
关于octopress建立博客小站的教程太多，
其实octopress本身的英文页面就介绍得挺详细的，
问题是一切顺利的广为人知的流程在搭完blog、显示出第一个hello world的simple post之后就结束啦，
怎么帖代码（教怎么高亮代码的倒是很多。。。），怎么贴图，怎么贴表格，怎么加粗加颜色删除线下划线……

<---- 咳，吐槽帝的需求的确比较麻烦，不符合hacker大人们的极简脑回路 - -|| 。。。
jekyll的英文页面看得实在头大，我几乎都想自己在文本里打&lt;/br&gt; 和 &lt;img&gt;&lt;/img&gt;了，咳。 

大概hacker们的思路太跳脱，这种小问题也需要解决么，文本编辑器里自己写去。。。
可是我等懒人实在受不了要么如此朴素的post要么如此复杂的输入啊喂。。。

这是一个零基础在octopress下，用各种手段发可爱的post的心路历程，只当学习吐槽了。
（refer to http://jekyllrb.com/docs/posts/ ）
<!--more-->
1、首先是换行，so easy 文本里两个回车（空一行）自动换行，和latex一样嘛

2、发高亮代码，和网上众多教程一样对代码高亮支持很好用法也简单：

效果拔群：
{% highlight ruby linenos %}
def show
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}

3、插入链接：