# 1.0 类和对象

[en-US](classes-and-objects.md)

# 1.1 何为类？ 何为对象？

前文便提到，Java是一门面向对象程序设计语言，而我们开始学习某一门语言，并不是仅仅只会编写程序而已，更要学会如何`设计`，而这样的`设计`的能力便是程序设计的美妙之处。

相信各位肯定也能在网络上查找到这样的`类`和`对象`的相关定义:

 - 类（Class）：定义了一件事物的抽象特点。类的定义包含了数据的形式以及对数据的操作。
 - 对象（Object）：是类的实例（Instance）。
 
不过，我们还需要区分`类`与`对象`的关系。
即：

> 类定义了对象，对象是由类所产生的，而同一个类所产生的对象不尽相同。

或者，你也可以用一个很显而易见的方法区分：

> 类并没有储存在内存空间中，而类只有实例化为对象才能作为对象储存在内存空间中。

# 1.2 抽象过程

我们需要进行抽象以是问题变成一个个类之间的问题，然后再通过类来解决问题。

在《Thinking in Java》书中，便有提到有Alan Kay总结的面向对象程序设计方式，与此同时，我们不妨来打个比方，比如我们现在有一辆车。

> **1.万物皆为对象。**<br>
> 车便是一个对象；你当然也是一个对象。
>
> **2.程序是对象的集合，它们通过发送消息来告知彼此所要做的。**<br>
> 这辆车和你共同所处的世界便是程序，你发动车子，便相当于向车子发送启动的消息。
>
> **3.每个对象都有自己的有其他对象所构成的存储。**<br>
> 车子中有发动机、底盘......；你也由消化系统、呼吸系统、运动系统......组成。 它们都是对象。
> 
> **4.每个对象都拥有其类型。**<br>
> 而车又是什么类型呢？它可以是机器，当然也可以就是车它本身。我们知道这里的机器和车都是类既然这个对象可以同时是两个类的实例，那么这两个类之间又有什么关系呢？别急！很快你就会在后面的`继承和多态`一章学到。
>
> **5.某一特定类型的所有对象都可以接受同样的消息。**<br>
> 是不是看到这句话就感觉有些不理解？不妨让我们再看看上一条，它可以是机器，当然也可以就是车它本身。当我们向具有`机器`这一类型的类发送信息时，我们的`车`类型的对象同时也可以接受其他类发往`机器`类的信息。这样的特性 我们称之为 `可替代性`，这是OOP语言的一个强有力的优势。