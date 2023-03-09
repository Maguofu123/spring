# day1
特点：  
IOC, AOP

Bean（容器）创建对象，加载配置文件时，对象已经创建了  
`value`具体的值，`ref`引用spring中创建好的对象

IOC创建对象方法：
1. 无参构造`id` `class` `property`
2. 有参构造`id` `class` `constructor-arg`

Spring配置：

# day2
import 导入其他xml文件

**依赖注入**
依赖：bean对象的创建依赖于容器  
注入：bean中对象的所有属性，由容器来注入
1. 构造器注入
2. set方式注入
3. 拓展方式注入

p命名空间，需要导入约束，直接设置字段参数，`p:`  
c命名空间，需要导入约束，通过构造器注入，`c:`

scope:单例模式（默认），原型模式（每次产生新对象），其他requset，session，application在web中应用

**bean自动装配**
1. 在xml中显式配置
2. 在java中显式配置
3. 隐式的自动装配bean （关键）

byName 寻找和set后面对应的值  
byType 和自己对象属性类型相同的bean

**注解自动装配**
1. 导入约束`xmlns:context="http://www.springframework.org/schema/context"` `http://www.springframework.org/schema/contex http://www.springframework.org/schema/context/spring-context.xsd"`
2. 配置注解支持`<context:annotation-config></context:annotation-config>`
3. 添加注解`@Autowired`，先byType，再byName

**注解开发**
`@component`放在组件上，即bean
1. dao @Repository
2. service @Service
3. controller @Controller


