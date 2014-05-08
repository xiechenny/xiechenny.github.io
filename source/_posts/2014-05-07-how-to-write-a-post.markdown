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
找了半天终于找到了markdown语法文档，也就是octopress默认生成的post文件所使用的解析方法了。
（http://daringfireball.net/projects/markdown/ ）
暂且一边看一遍挑常用的列一列。

<!--more-->
1、首先是换行，so easy 文本里两个回车（空一行）自动换行，和latex一样嘛

2、发代码，用法也简单，代码块前面集体加tab缩进，效果：

	def show
	  @widget = Widget(params[:id])
	  respond_to do |format|
		format.html # show.html.erb
		format.json { render json: @widget }
	  end
	end



3、引用，每段开头加&gt;：

代码：

— — — — — — — — — — — — — — — — — — —

&gt; 我是引用，blablabla...

— — — — — — — — — — — — — — — — — — —


效果：
>我是引用，blablabla...

4、斜线、加粗， (*和_的作用是一样的)：
	*我加了<em>标签*			_我加了<em>标签_
	**我加了<strong>标签**		__我加了<strong>标签__
*我加了&lt;em>标签*

**我加了&lt;strong>标签**

5、支持的html标签:	&lt;div>, &lt;table>, &lt;pre>, &lt;p> 

6、link ：
	[link](http://url.blablabla...)
7、图片
	![Alt text](/path/to/img.jpg "Optional title")

Last、不是tips的tips：

需要用符号如“-”手动绘制一些边线的时候可以选用全角符号，就不会被默认语法错误识别了。

（咳，双线程，一遍研究c++ 一遍研究octopress 写得比较慢。。。）