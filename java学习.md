# java学习

## 一、基础

### 1.4算法分析

#### String

    public final class String（大概）
	{
		private final char[] value; // 字符数组存放字符空间，子字符串公用
		private int offset;	  // 偏移量，子字符串中有用到
		private int count;    // 计数器（字符串长度）
		private int hash;     // 存放字符串的哈希值，串相同时，这个值也相同
	...
	}

字符串和它的子字符串重用相同的value[]数组。

String对象不可变。

#### 内存分配

对象保存在堆上，原始数据类型和对象引用保存在栈上

#### 数组

    int[] a = new int[N]

大多数情况下，有N次的数组访问（初始化为零）。

## 二、排序

### 2.1初级排序算法

#### Comparable接口、compareTo方法

可比较的数据类型要实现Comparable接口中的compareTo()方法。
对于v<w,v=w和v>w，java习惯在调用v.compareTo(w)是返回（-1、0和1）

