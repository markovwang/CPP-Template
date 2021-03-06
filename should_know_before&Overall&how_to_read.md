# 读前须知



为了让读者能够较好的从本书有所收获, 读者应该有一定的C++基础, 在此书中, 我们将详细地讲解一些语言的特性, 而非讲解语言的基础, 那些类啊, 继承啊啥的概念你好歹得熟悉吧, 并且好歹会用标准库的IO流吧.当然, 这本书面向`C++11, C++14, C++17`, 所以现代C++中的那一套比如`auto`,`decltype`关键字啊,移动语义啊, lambda表达式啊, 总得会点吧.

不过, 即使有必要 ,我们也会根据需要审查更细微的, 与模板没有直接关系问题. 这也使得这本书不仅面向专家, 也面相中级程序员. 

此书中主要涉及C++11, C++14, C++17的标准, 当然, 此书做成时,C++17标准尚未尘埃落定. 我们希望读者不会很快就对这些细节了如指掌. 所有的修订版均对模板有深厚的影响. 因此我们会给与我们主题强烈相关的新特性加以简短的说明. 不过, 之前说过, 我们的目标并非介绍现代标准, 也非给出一个从上古C++到现代C++的详细描述.相反, 我们关注于C++设计且使用的模板, 以现代C++为基础, 也会偶尔给出一些案例, 即现代C++标准允许或提倡和之前不同的做法.





# 全书总览



我们的目的是提供一些开始使用模板的必要信息, 并希望你从借模板之力从中获益. 并似的身经百战的程序员更上一层楼.为了达到此目标, 我们决定将本书分为以下几*部分*.

- **第一部分**: 讲解模板的基础概念, 并且是以教程的风格写作而成.
- **第二部分**: 呈现语言细节, 并且能够让程序员将此章节作为模板相关代码结构的趁手参考.
- **第三部分**: 阐述C++模板的基本设计于代码技巧, 从最基础的写法到你想不到的奇技淫巧之代码, 应有尽有.

每一章均包含数节, 另外, 我们还附赠了一个附录, 里面讲了些除了模板外其他的东西. 其中有一章讲解了`concepts`, 是(当时)C++20草案中对模板的一个延伸.(此书出版时`concepts`已经成为C++20标准中的一部分).

第一部分的那些章节按照次序读比较好, 比如第三章依赖第二章的内容.而其他章节之间的联系要松散一些.交叉引用能使得读者更好的在各章节之间蹦跶.

最后, 我们提供了一个相当完整的索引, 鼓励以其他方式不按顺序阅读这本书. 



# 如何阅读此书

如果是一个想学习或复习一下模板的概念, 建议仔细阅读第一部分. 就算你已经对模板烂熟于心, 快速略读此部分亦可以让你熟悉我们的变成风格于术语.这一章也包含一些当你使用模板时如何组织源代码的方面.

取决于你的学习方法, 你可以选择吸收第二部分中的哪些知识点, 或者, 你可以去阅读第三部分关于实践的内容(并回去参考第二部分中一些问题的精妙解释). 第二种阅读方法尤其的巧--如果你是买来本书并记得天天给自己一些挑战的话.

附录包含了很多有用的信息, 而它们绝大部分在正文中都会参考到. 我们也在保证正确的前提下写得有趣一些.

按照我们的经验, 学习一些新东西是最好的方法是通过例子来学习, 因此你能在本书中找到很多例子, 一些例子区区几行,即介绍一些概念, 同时也有一些完整的程序给出某个内容的具体应用. 后一种可以在代码的注释中看到详细的说明.

你可以在下面的网站中找到本书代码:

[http://www.tmplbook.com](http://www.tmplbook.com)

