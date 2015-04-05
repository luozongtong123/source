layout: post
title: "Python 中需要注意的点"
toc: true
date: 2015-03-27 19:39:49
tags: 知识管理
category: Python
description: 将在学习 Python 时遇到的问题在此记录一下。
---

python 中数据分为可变对象，和不可变对象。
* 不可变对象：int，string，float，tuple
* 可变对象   ：list，dictionary
在函数传递参数时，若传递的是不可变对象则函数获得的是不可变对象的值，而如果传递的是可变对象则函数获得的是可变对象的地址(类似 C 语言的指针)。利用这个特点可以方便的利用参数返回计算结果，但是同时需要注意： **在函数中使用可变对象一定要注意在循环中的可变对象的初始化，防止多个循环造成数据混乱。**