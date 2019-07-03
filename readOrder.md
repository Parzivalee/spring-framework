### Spring Framework的架构
1. Core Container：包括Core、Beans、Context 和Expression Language模块。
其中，Core和Beans是框架的基础部分，提供IoC(控制反转)和依赖注入的特性。
* Core模块主要包括Spring框架的核心工具类，Spring的其它组件都要用到这个包里的类，Core模块是其它组件的基本核心。
* Beans模块是所有应用都要用到的，它包含访问配置文件、创建和管理bean以及进行IoC/DI操作相关的所有类。
* Context构建于Core和Beans之上，提供了一种类似于JNDI注册器的框架式的对象访问方法。Context模块继承了Beans的特性，为Spring核心提供了大量的拓展，包括对国际化（例如资源绑定）、事件传播、资源加载和对Context的透明创建的支持。ApplicationContext接口是Context模块的关键。
* Expression Language模块提供了强大的表达式语言，用于在运行时查询和操纵对象。它是基于JSP2.1规范中的unifed expression language的拓展。