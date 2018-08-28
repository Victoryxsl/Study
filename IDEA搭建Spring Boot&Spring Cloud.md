---
typora-root-url: IDEA搭建Spring Boot&Spring Cloud
---

##IDEA搭建Spring Boot&Spring Cloud

  

> 使用IDEA搭建Spring-Boot项目

###介质安装

####安装完成后

+ 创建新的项目
+ 导入已经创建的项目(通过.grade,.project,.pom加载项目)
+ 打开项目文件夹
+ 检出版本控制的项目(github,GIT,CVS)

####导入已存在的项目

地址：<http://spring.io/guides/gs/spring-boot/>

1. 下载demo例子

![1](1.png)

​	2. 导入项目可以选择pom直接导入(maven项目)

**搭建Springboot以及后续的Springcloud要使用JDK1.8以上版本**

![2](2.png)

导入项目后,当前工程会通过默认的IDEA自带Maven配置来下载项目的相关依赖(Dependency Types)

这个配置会自动获取当前项目的依赖包进行下载（依赖关系存在于项目的管理文件pom.xml）

其中开始下载第一个依赖 spring-boot-starter-parent

![image021](/image021.png)



在复合项目多模块管理时，作为父项目可以不生成包文件。

如下图,打包方式就是pom,作用是提供依赖和插件的管理,它还有父项。通过父项的GAV再往上查找下载

![image056](/image056.png)

查看父项

![image058](/image058.png)



所有springBoot的依赖关系在这个文件中表示

其中src指向的就是spring-boot的源码地址，代码的更新和版本的迭代就是GAV的控制。

![image060](/image060.png)



#### 运行项目

项目已经没有报错了，验证下spring官网提供的spring-boot例子

选中application点击运行

![image101](/image101.png)

Spring-boot内置了tomcat，详细的spring-boot信息自行学习。

![image103](/image103.png)

![image107](/image107.png)

查看rest接口请求

![image109](/image109.png)

Spring官网的springboot的例子已经搭建完毕，可以在这个demo的基础上开发，也可以去官网查看更多的spring-boot项目的例子

进行学习并实践。但是如果需要创建新的SpringBoot项目，则如下所示，因为需要了解依赖模块的东西，所以一般先从demo入手学习

比较快，有了一定的基础就可以直接构建项目。
