# Part Ⅰ



## The Basics

这一部分主要介绍基本概念和C++的模板特性. 这一部分以函数模板和类模板为例, 来展示我们的目标和基本概念.然后又添加了一些基本模板特性比如无类型参数模板, 变长模板, `typename`关键字, 成员模板. 而且讨论了如何处理移动语义, 如何生命参数, 并且如何在编译期编程中使用模板. 最后是一些关于术语的一般性提示, 即对编程人员有用, 对于泛型库的作者也颇有帮助.



## 为何选择模板?

C++ 中当我们去定义变量, 函数, 以及其他的大多数实体的时候, 都要使用具体的类型, 然而, 很多代码除了类型不同, 看起来大致一样, 就比如, 当我们实现快排算法的时候, 对于不同的数据结构, 程序的接口看起来是相同的, 比如整形的数组啊, 字符串组成的向量啊, 他们都包含着可以相互比较的类型.

如果你的编程语言并不能支持这种泛型的话, 你只能用很糟糕的替代方法了:

1. 对于不同的类型, 把同一种行为实现一遍又一遍.
2. 或者是使用`void*`或者是`Object`来实现不优雅的泛型.
3. 可以使用特化预处理器.

如果你是从别的语言那边来的, 可还真可能整过这一出, 但是, 上面这三种方法都有其缺点:

1. 把同一种行为写了一遍又一遍, 呃...这不就是造轮子吗? 你会犯同样的错误, 然后你倾向去避免复杂但是更好的算法, 因为这会让你犯更多的错,
2. 如果你为基于某一个基类的类型写同样的代码, 你便无法享受到类型检查带来的益处. 并且, 一些类可能是由特定的基类继承而来, 这样你的代码将十分难以维护.
3. 你用预处理器的话, 恭喜你, 你将使用"脑瘫的文本替换机", 这时你根本没办法检查什么作用域啊, 类型啊, 这可能会导致乱七八糟的语义错误. 

而我们亲爱的模板能够解决以上所有问题, 并且不会带来任何问题, 模板可以是尚未指定一种或多种类型的函数或者类. 当你使用模板的时候, 你可以以显式或者隐式的方法把类型本身当作参数传入. 因为模板是语言特性, 所以编译器会帮你做好作用域和类型检查的.

如今的程序中, 模板已经被大规模使用, 举个例子, 在C++标准库中, 几乎全部代码用到了模板, 标准库提供了可以用来对特定类型的值, 管理特定类型的数据结构(也叫容器), 字符串来进行排序. 然而,  这仅仅是开始, 模板甚至允许我们参数化行为, 来优化代码, 也可以参数化数据. 这些稍微高级一些的代码将在稍后的章节覆盖到, 咱们先看点简单的模板吧.