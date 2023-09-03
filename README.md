设计模式的分类
一、总体来说设计模式分为三大类：

创建型模式，共五种：工厂方法模式、抽象工厂模式、单例模式、建造者模式、原型模式。

结构型模式，共七种：适配器模式、装饰器模式、代理模式、外观模式、桥接模式、组合模式、享元模式。

行为型模式，共十一种：策略模式、模板方法模式、观察者模式、迭代子模式、责任链模式、命令模式、备忘录模式、状态模式、访问者模式、中介者模式、解释器模式。

二、三类设计模式的区别
创建型模式、结构型模式和行为型模式是三种不同类型的设计模式，它们在软件设计中有不同的应用和职责。

1. **创建型模式**：
   - 主要关注对象的创建机制，以确保系统中的类实例化过程更加灵活、可扩展和封装。
   - 创建型模式包括单例模式、工厂模式、抽象工厂模式、建造者模式和原型模式。
   - 用于解决对象的创建、初始化和管理问题。

2. **结构型模式**：
   - 主要关注对象之间的组合和组装，以构建更大的结构，同时保持结构的灵活性。
   - 结构型模式包括适配器模式、桥接模式、组合模式、装饰器模式、外观模式、享元模式和代理模式。
   - 用于解决对象的组织和协作问题，以实现更好的代码复用和系统的可维护性。

3. **行为型模式**：
   - 主要关注对象之间的通信、交互和责任分配，以定义对象之间的行为。
   - 行为型模式包括策略模式、模板方法模式、观察者模式、迭代器模式、责任链模式、命令模式、备忘录模式、状态模式、访问者模式和中介者模式等。
   - 用于解决对象之间的交互和协作问题，以实现更灵活、可维护和可扩展的系统。

总结：
- 创建型模式关注对象的创建，结构型模式关注对象的组织，行为型模式关注对象的行为。
- 创建型模式用于处理对象的创建过程，结构型模式用于处理对象之间的组织关系，行为型模式用于处理对象之间的交互和行为。
- 各种设计模式在不同的情景下都有各自的用途，选择合适的设计模式取决于问题的性质和需求。



golang中的应用
在 Go（或称为 Golang）中，虽然设计模式并不像在某些其他编程语言中那么显式，但仍然可以应用设计模式的原则，尤其是一些基本的设计模式。以下是一些在 Go 中常见的设计模式和它们的应用情况：

1. **单例模式（Singleton Pattern）**：确保一个类型只有一个实例。在 Go 中，可以使用包级别的变量和`sync.Once`来实现单例模式。

2. **工厂方法模式（Factory Method Pattern）**：定义一个接口来创建对象，但让子类决定具体实例化哪个类。Go 中经常使用工厂函数来创建对象。

3. **策略模式（Strategy Pattern）**：定义一系列算法，将它们封装起来，并且使它们可以互相替换。Go 中使用函数作为一等公民，可以轻松实现策略模式。

4. **观察者模式（Observer Pattern）**：定义了一种一对多的依赖关系，当一个对象状态发生变化时，所有依赖它的对象都会得到通知并更新。Go 中可以使用回调函数或通道来实现观察者模式。

5. **装饰器模式（Decorator Pattern）**：动态地给一个对象添加一些额外的职责。Go 中使用组合和包装函数可以实现类似装饰器模式的效果。

6. **适配器模式（Adapter Pattern）**：将一个接口转换成另一个客户希望的接口。Go 中经常使用接口来实现适配器。

7. **命令模式（Command Pattern）**：将请求封装成一个对象，从而可以参数化其他对象，将请求排队或记录请求日志，以及支持可撤销的操作。Go 中可以使用函数和闭包来实现命令模式。

8. **模板方法模式（Template Method Pattern）**：定义一个算法的骨架，但将一些步骤延迟到子类中。在 Go 中，可以使用匿名字段和接口来实现类似的效果。

虽然 Go 中的设计模式可能不如其他语言那么突出，但由于 Go 的简洁性和面向接口的设计，很多设计模式在 Go 中以更简洁的方式实现。开发人员通常倾向于使用更自然的 Go 风格来解决问题，而不一定非要遵循传统的设计模式。不过，了解这些模式的概念和原则仍然对编写清晰、可维护的 Go 代码有帮助。