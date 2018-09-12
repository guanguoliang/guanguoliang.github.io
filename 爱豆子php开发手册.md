# 一、编程规约
## （1）命名风格

 1. 【强制】代码中的命名均不能以==下划线== 开始，也不能以==下划线==结束。 <br>反例：`_name / __name /  name_ / name__`
 2. 【强制】代码中的命名严禁使用拼音与英文混合的方式，更不允许直接使用中文的方式。 说明：正确的英文拼写和语法可以让阅读者易于理解，避免歧义。注意，即使纯拼音命名方式 也要避免采用。<br> 正例：alibaba / taobao / youku / hangzhou 等国际通用的名称，可视同英文。 <br>反例：DaZhePromotion [打折] / getPingfenByName() [评分] /  某变量 = 3
 3. 【强制】类名使用 UpperCamelCase 风格，但以下情形例外：DO / BO / DTO / VO / AO / PO / UID 等。<br> 正例：MarcoPolo / UserDO / XmlService / TcpUdpDeal / TaPromotion <br>反例：macroPolo / UserDo / XMLService / TCPUDPDeal / TAPromotion
 4. 【强制】方法名、参数名、成员变量、局部变量都统一使用 lowerCamelCase 风格，必须遵从 驼峰形式。 <br>正例： localValue / getHttpMessage() / inputUserId
 5. 【强制】常量命名全部大写，单词间用下划线隔开，力求语义表达完整清楚，不要嫌名字长。 <br>正例：MAX_STOCK_COUNT <br>反例：MAX_COUNT
 6. 【强制】抽象类命名使用 Abstract 或 Base 开头；异常类命名使用 Exception 结尾；测试类 命名以它要测试的类的名称开始，以 Test 结尾。
 7. 【强制】杜绝完全不规范的缩写，避免望文不知义。<br> 反例：AbstractClass“缩写”命名成 AbsClass；condition“缩写”命名成 condi，此类随 意缩写严重降低了代码的可阅读性。
 8. 【推荐】为了达到代码自解释的目标，任何自定义编程元素在命名时，使用尽量完整的单词 组合来表达其意。<br><font color='green'> 正例</font>：表达原子更新的类名为：AtomicReferenceFieldUpdater。<br><font color='red'> 反例</font>：变量 int a 的随意命名方式。
 9. 【推荐】如果模块、接口、类、方法使用了设计模式，在命名时需体现出具体模式。 说明：将设计模式体现在名字中，有利于阅读者快速理解架构设计理念。 <br><font color='green'>正例</font>：class OrderFactory; <br> class LoginProxy; <br> class ResourceObserver;
 10.接口和实现类的命名有两套规则：<br> 1）【强制】对于 Service 和 DAO 类，基于 SOA 的理念，暴露出来的服务一定是接口，内部 的实现类用 Impl 的后缀与接口区别。 <br><font color='green'>正例</font>：CacheServiceImpl 实现 CacheService 接口。 <br>2）【推荐】如果是形容能力的接口名称，取对应的形容词为接口名（通常是–able 的形式）。<br> <font color='green'>正例</font>：AbstractTranslator 实现 Translatable 接口。 

> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTY0MTQ5NjczN119
-->