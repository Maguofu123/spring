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
