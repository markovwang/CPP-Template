# C++ Templates 中翻(第二版)



翻译这本书的契机呢, 是我在写一个软渲染引擎, 里面有一些矩阵运算, 一开始打算用`eigen`, 而`eigen`编译奇慢, 而`DirectXMath`又不跨平台, 想自己写个矩阵库顺便练练手, 也想玩玩编译期编程 (露出了菜狗的目光

发现我原先写的C++完全是`C with Classes`, 对于模板或者是元编程实在是生疏.

而这本书也买不到中文版, 于是一边写矩阵库一边看这本书, 顺便翻一下.

这本书说实话有点过于详细了, 如果对于C++模板一窍不通的话, 我认为在看过`Effective Modern C++`的基础上看下来是没有问题的.





## 译者 24岁, 是学生, 喜欢玩王道征途

## 女朋友是嘤岛麻衣 !!!

## 是一个在二流211的二流研(班)究(儿)生(逼)

## 所以翻译得很慢

## 如果翻译有误请在issue区提出



#### 翻译不完了, 心态炸了, 嘤嘤嘤.







## 目录及翻译进度:



关于本书

​	读前须知

​	本书结构

​	如何读本书

​	编程风格说明

​	C++11 C++14 C++17 标准

​	示例代码与额外信息

​	反馈

Part 1: 基础

1. 函数模板

   √1.1 初见函数模板	

   √1.2 模板实参推断

   √1.3 多模板参数

   √1.4 默认模板实参

   √1.5 重载函数模板

   √1.6 该... 还是不该?

   √1.7 总结

2. 类模板

   √2.1 Stack类模板的实现

   √2.2 使用Stack的类模板

   √2.3 类模板的部分使用

   √2.4 友元

   √2.5 类模板的特化

   √2.6 偏特化

   √2.7 默认类模板实参

   √2.8 类型别名

   √2.9 类模板实参推断

   √2.10 模板化聚合

   √2.11 总结

3. 非类型模板参数

   √3.1 非类型类模板参数

   √3.2 非类型函数模板参数

   √3.3 非类型模板参数的限制

   √3.4 auto非类型模板参数

   √3.5 总结

4. 变长模板

   √4.1 变长模板

   ​	√4.1.1 举例变长模板

   ​	√4.1.2 重载变长和非变长模板

   ​	√4.1.3 sizeof ...运算符

   √4.2 折叠表达式

   √4.3 使用变长模板

   √4.4 变长雷模板和变长表达式

   ​	√4.4.1 变长表达式

   ​	√4.4.2 变长索引

   ​	√4.4.3 变长类模板

   ​	√4.4.4 变长推断指引

   ​	√4.4.5 边长基类及其使用

   √4.5 总结

5. 基础技巧

   √5.1 `typename`关键字

   √5.2 零初始化

   √5.3 使用`->this`

   √5.4 裸数组和字符串字面量的模板.

   √5.5 成员模板
   
   ​	√5.5.1 .template的使用
   
   ​	√5.5.2 泛型lambda和成员模板
   
   √5.6 变量模板
   
   √5.7 模板模板参数
   
   √5.8 总结

​	6. 移动语义和`enable_if<>`

