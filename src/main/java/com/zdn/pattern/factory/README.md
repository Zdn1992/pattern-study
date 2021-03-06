# 工厂模式
---
>From CSDN @LSZJXin 
1. 简单工厂
2. 工厂方法
3. 抽象工厂

---
### UML类图
* 简单工厂   
![staticmethod](https://github.com/Zdn1992/pattern-study/blob/master/src/main/java/com/zdn/pattern/factory/staticmethod/uml/staticmethod.png)
* 工厂方法   
![method](https://github.com/Zdn1992/pattern-study/blob/master/src/main/java/com/zdn/pattern/factory/method/uml/method.png)
* 抽象工厂   
![abstract](https://github.com/Zdn1992/pattern-study/blob/master/src/main/java/com/zdn/pattern/factory/abstractmethod/uml/abstractmethod.png)
### 总结
* 通过UML图以及代码不难对三种工厂模式进行一个区分。简单工厂模式，工厂类是整个模式的关键所在，包含了必要的逻辑判断，能够外界给定的信息， 决定究竟创建哪个具体类的对象。工厂方法模式 是对简单工厂方法模式的一个抽象，抽离出了一个Factory类(或者接口)，这个接口不负责具体产品的生产，而只是指定一些规范，具体的生产工作由其子类去完成。这个模式中，工厂类和产品类往往是一一对应的，完全解决了简单工厂模式中违背“开闭原则”的问题，实现了可扩展；抽象工厂模式 的特点是存在多个抽象产品类，每个抽象产品类可以派生出多个具体产品类，工厂提供多种方法，去生产“系列”产品。

* 简单工厂模式适用于工厂类需要创建的对象比较少的情况，客户只需要传入具体的参数，就可以忽略工厂的生产细节，去获取想要的对象；工厂方法模式，主要是针对单一产品结构的情景；抽象工厂模式则是针对多级产品结构(系列产品)的一种工厂模式。最后在说一下，每种模式都有自己的优点和弊端，没有最好的模式，只有最适合的模式，只要符合实际开发需求就是最好的。

