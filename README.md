# TransferAccountSystem5.0
相比4.0增加代理模式，将service层的事务操作放到代理类实现
#	代理模式的创建步骤
#1）	创建业务接口，在业务接口中，写业务方法
#2）	完成接口的真正实现类，实现接口，重写方法，完成方法体
#3）	完成接口的代理实现类，实现接口，重写方法
a.	写成员变量，类型为真正的实现类
b.	写带有一个参数的构造方法，代替原来默认的无参构造方法，参数类型为真正的实现类，由该参数为成员变量赋值
c.	代理实现类的业务方法由两部分内容来完成，第一部分内容：使用成员变量完成业务逻辑，第二部分内容：业务逻辑的扩展
#4）在使用的过程中，先创建真正的实现类对象，再创建代理实现类对象，最后我们用就用代理实现类的对象
