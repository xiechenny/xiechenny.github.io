---
layout: post
title: "JAVA程序员从零开始学习C++"
date: 2014-05-08 15:42:54 +0800
comments: true
categories: c++
---
作为一个本科期间只系统学过JAVA的程序员，
虽然至今为止多多少少也已经修改并优化过许多基于c++的开源程序，
相关书籍也多多少少看了一些，但终归不成系统。
因为网易实习的c++并linux编程环境需求，
终于决定以greedy snake为例从零开始学习build c++ project ^ ^.

基本构思很简单：
一个main函数，一个game class(维护地图)， snake class；
输出基于命令行，学习一下CJ推荐的courses库；
先不做用户交互，直接写自动运行版的贪吃蛇，一秒钟走一步。

于是从零开始！

第一步，自己配置vim，
参考bbs精华帖，手把手教你把vim配置成IDE 
（http://bbs.sjtu.edu.cn/bbs0an,path,%2Fgroups%2FGROUP_3%2FGNULinux%2FSoftware%2FD95E89182%2FD5277E56B.html ）
教程比较长，先配置到ctags，
snake project起步时文件还较少，后面的文件资源管理暂且边写边学习也不会太枯燥。
<!--more-->

【重要tips】配置.vimrc时需要额外注意tab键功能相关的设置,
由于makefile在build target时会根据tab键来识别需要执行的编译命令，
所以在vim中开启一些tab键与空格转换之类的操作，会引起后面make file编写失败！

第二步， 从零开始编写Makefile！


