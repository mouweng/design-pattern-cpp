# 设计模式（c++实现）

------



## 设计模式原则

### 单一职责原则

> 就一个类而言，应该仅有一个引起它变化的原因

- 如果一个类承担的职责过多，就等于把这些职责耦合在一起，一个职责的变化可能会削弱或抑制这个类完成其他职责的能力。这种耦合会导致脆弱的设计，当变化发生时，设计会遭受到意想不到的破坏

- 软件设计真正要做的许多内容，就是发现职责并把哪些职责相互分离

- 判断一个是否应该分离出类来：如果你能够想到多于一个的动机去改变一个类，那么这个类就具有多于一个职责

### 开放封闭原则（核心原则）

> 对于软件实体（类、模块、函数等）的扩展是开放的，对于软件实体的更改是封闭的

- 面对需求，对程序的改动那个是通过增加新代码进行的，而不是更改现有的代码。

- 开发人员应该仅对程序中呈现出频繁变化的哪些部分作出抽象，然而，对于应用程序中的每一个部分都刻意进行抽象同样不是一个好主意。拒绝不成熟的抽象和抽象本身一样重要！

### 倒转依赖原则（贯穿所有模式）

> 高层模块不应该依赖于底层模块，两个都应该依赖于抽象
>
> 抽象不应该依赖细节，细节应该依赖抽象

![](https://tva1.sinaimg.cn/large/006y8mN6gy1g8xlp77hkxj30ms0doq3f.jpg)

说白了就是要针对接口编程，不要对实现编程



### 里式替换原则

> 子类必须能够替换他们的基类（is-a）

只有当子类可以替换掉父类，软件单位的功能不受到影响时，父类才能真正被复用，而子类也能够在父类的基础上增加新的行为。



### 接口隔离原则（ISP）

> 不应该强迫客户程序依赖他们不用的方法
>
> 接口应该小而完备



### 优先使用对象组合，而不是类继承

> 继承在某种程度上破坏了封装性，子类父类耦合度高
>
> 对象组合则只要求被组合的对象具有良好定义的接口，耦合度低



### 封装变化点

> 使用封装来创建对象的分界层，让设计者可以在分界层的一侧进行修改，而不会对另一侧产生不良的影响，从而实现层次间的松耦合



### 针对接口编程，而不是针对实现编程

> 不将变量类型声明为某个特定的类，而是声明为某个接口
>
> 客户程序不需知道对象具体类型，只需要知道对象的接口
>
> 减少系统中各部分的依赖关系



------



## 设计模式类别

### 一、简单工厂

简单工厂是由一个抽象产品类和一个具体工厂类实现的；

![](https://tva1.sinaimg.cn/large/006y8mN6gy1g8wenh6regj310u0l2410.jpg)

面向对象的编程，并不是类越多越好，类的划分是为了封装，单分类的基础是抽象，具有相同属性和功能的对象的抽象集合才是类。

### 二、策略模式





