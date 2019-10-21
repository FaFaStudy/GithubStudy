# Github实战项目学习
#### 一、电商项目 https://github.com/macrozheng/mall
#### 二、SwaggerAPI文档转Word文档的工具 https://github.com/JMCuixy/swagger2word
#### 三、Springboot学习 https://github.com/Snailclimb/springboot-guide
###### 1、Springboot介绍与开发环境搭建
###### 2、Springboot入门HelloWorld
###### 3、Restful服务与Lombok插件
RESTful Web 服务与传统的 MVC 开发一个关键区别是返回给客户端的内容的创建方式：
传统的 MVC 模式开发会直接返回给客户端一个视图，
但是 RESTful Web 服务一般会将返回的数据以 JSON 的形式返回，这也就是现在所推崇的前后端分离开发。
使用 Lombok 来优化 Java 代码，以及一些开发 RestFul Web 服务常用的注解

@RestController vs @Controller
单独使用 @Controller 不加 @ResponseBody的话一般使用在要返回一个视图的情况，这种情况属于比较传统的Spring MVC 的应用，对应于前后端不分离的情况。
@RestController返回JSON或XML形式数据
但@RestController只返回对象，对象数据直接以 JSON 或 XML 形式写入 HTTP 响应(Response)中，这种情况属于 RESTful Web服务，这也是目前日常开发所接触的最常用的情况（前后端分离）。
###### 4、热部署
添加依赖和插件
	<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-devtools</artifactId>
      <scope>runtime</scope>
			<optional>true</optional>
		</dependency>
    
    <plugin>
     <groupId>org.springframework.boot</groupId>
     <artifactId>spring-boot-maven-plugin</artifactId>
  </plugin>

