---
layout: post
title:  "Gradle学习之Groovy"
date:   2018-07-09 15:08:32
categories: Gradle Groovy
---
### 1. Groovy简介
>Groovy与java类似，都在java虚拟机中运行，当运行Groovy脚本时它会被先编译成java类字节码。
>Groovy需配置环境变量，压缩包下载地址：http://www.groovy-lang.org/download.html，在Path环境变量中加上bin目录的路径，通过groovy -version命令检查是否配置成功。

### 2. Groovy语法
* 单引号对应字符串，不对内容进行转义
* 双引号内容类似脚本，会对内容进行转义
```groovy
def x = 100
def s1 = "i am $x dolloar"
println( s1 )
```
>结果：
    i am 100 dolloar
* 三引号类似文本框，字符串中可随意换行
* 定义变量和函数用def关键字，函数如果有返回值，则可以不用def关键字
* 如不用return，则函数最后一行代码为返回值
* 函数调用可不加括号
* 断言assert
>断言变量的长度
```
def s2 = "abc"
assert s2.size()>3
```
* for循环
>输出5个
```
for (i in 0..<5){
    println("hello world")
}
```
* time循环
>循环4次（0,1,2,3）
```
4.times {
    println it
}
```
