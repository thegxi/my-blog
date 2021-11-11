---
title: javascripts
date: 2021-10-27 17:33:36
tags:
---
##### javascripts引擎
- V8: Chrome和Opera中的js引擎
- SpiderMonkey: Firefox中的js引擎
- Chakra: IE中的js引擎
- SquirrelFish: Safari中的js引擎
##### 变量提升
####### Javascript在预编译期会先预处理声明的变量,但是变量的赋值操作发生在JavaScript执行期,即声明变量即使放到最后,由于Javascript在预编译期已经对变量声明语句进行了预解析;
```javascript
document.write(str); //显示undefined
str = http://c.biancheng.net/js/;
document.write(str); //显示 http://c.biancheng.net/js/
var str;
```
##### let和const
- let: 声明的变量只在其所在的代码块中有效,且在代码块中不能重复声明
- const: 功能与let相同,只是const定义的变量一量定义就不能更改,即const定义的变量称为常量
