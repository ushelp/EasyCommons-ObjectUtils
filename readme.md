# EasyObjectUtils 项目简介

---------------


EasyObjectUtils 是 EasyCommons 项目组下的对象操作组件。

> [EasyCommons](https://github.com/ushelp/EasyCommons "EasyCommons") 一个针对Java开发领域提供通用开发组件的项目。旨在为Java项目开发领域并不完善的一些方面，提供一些组件级的解决方案。
> 该项目有多个子项目，会不断收集相关组件，也欢迎有新的组件加入。



EasyObjectUtils is EasyCommons project group obejct operations component. 

>  [EasyCommons](https://github.com/ushelp/EasyCommons "EasyCommons") is a development component to provide a common field for Java development projects. Java is designed to develop programs in the field of some aspects of the project is not perfect, some component-level solutions.
>  The project has multiple sub-projects, will continue to collect related components, also welcomed the new components added.



## 中文

- **EasyObjectUtils 核心**

 1. **EasyObjectExtract**：对象抽取。 从对象中使用字段表达式(`FieldExpression`)抽取指定属性以 **key-value** 存入Map集合。 
 
 **适合场景**：JSON输出时，从对象中抽取指定输出属性和值。 
 
 2. **EasyObjectFilter**：JavaBean对象属性过滤。将对象中的特殊字符(<,>,...)全部过滤掉，转为转义符；或者自定义字符转换映射。 
 
 **适合场景**：将JavaBean对象属性中的字符串包含的特殊字符进行过滤转换为字符实体；或将对象字符串属性中包含的字符全部替换为指定字符。例如，在Struts2中文件上传时提交的数据封装到对象后，对对象中可能包含的用户提交的的特殊字符串的进行转义。
 
 3. **EasyObjectSetNull**：对象属性置空。使用字段表达式(`FieldExpression`)将对象中指定属性设置为null。 

 **适合场景**：将Hibernate加载的对象中有些延迟无法加载的属性设置为空 ，防止在序列化属性时出现no session异常。

- **EasyObject FieldExpression（字段表达式）语言**
 可以在进行对象操作时进行属性定位。
 ```
  指定属性： property 
  指定属性的属性：property.property
  指定集合中每一个对象： {collection}
  指定数组中每一个对象： [array] 
  指定集合中每一个对象的属性：{collection}.property 
  指定数组中每一个对象的属性：[array].property 

  别名定义(仅适用于EasyObjectExtract)：FieldExpression#Alias
 ```

[EasyObjectUtils API - 中文](doc/API-zh.md "EasyObjectUtils API")

[官方主页](http://www.easyproject.cn/easycommons/zh-cn/index.jsp '官方主页')

[留言评论](http://www.easyproject.cn/easycommons/zh-cn/index.jsp#donation '留言评论')

如果您有更好意见，建议或想法，请联系我。


## English

- **EasyObjectUtils core:**

 1. **EasyObjectExtract**: extraction of the object. Using field expression from the object (`FieldExpression`) to extract the specified property deposited **key-value** Map collection.<br/>
  **Scene**: JSON output, specify the output attributes and values extracted from the object.
 
 2. **EasyObjectFilter**: JavaBean Object property filtering. The object of special characters (<,>, ...) to filter out, into the escape character; or custom character transformation maps.<br/>
 **Scene** : the special character JavaBean Object property contains a string to filter into character entity; or a character string property objects included replacing all the specified character. For example, the data in the file upload Struts2 package submitted to the object, a special string to the user object may contain submitted escaped.
 
 3. **EasyObjectSetNull**: Object Properties empty. Using field expressions  Language(`FieldExpression`) specified property set to null object.<br/>
 **Scene**: Hibernate object loaded some delay attribute set can not be loaded is empty, to prevent abnormal when no session serialized property.

- **EasyObject FieldExpression language**
 EasyObjectUtils the tools used to **EasyObject FieldExpression (field expression) language** for property positioning when you operate object.
 
 Syntax:
  ```
  Specified attributes: property
  Specify the attribute that: property.property
  Each object in the specified collection: {collection}
  Each object in the specified array: [array] Attribute specifies for each object in the collection: {collection} .property
  Attribute specifies for each object in the array: [array] .property
  
  Alias definitions (only for EasyObjectExtract): FieldExpression#Alias
  ```

[EasyObjectUtils API - English](doc/API-en.md "EasyObjectUtils API")

[The official home page](http://www.easyproject.cn/easycommons/en/index.jsp 'The official home page')

[Comments](http://www.easyproject.cn/easycommons/en/index.jsp#donation 'Comments')

If you have more comments, suggestions or ideas, please contact me.


## Maven
```XML
<!-- EasyObjectUtils -->
<dependency>
	<groupId>cn.easyproject</groupId>
	<artifactId>easycommons-object</artifactId>
	<version>1.7.4-RELEASE</version>
</dependency>
```

## End

[官方主页](http://www.easyproject.cn/easycommons/zh-cn/index.jsp '官方主页')

[留言评论](http://www.easyproject.cn/easycommons/zh-cn/index.jsp#donation '留言评论')

[The official home page](http://www.easyproject.cn/easycommons/en/index.jsp The official home page')

[Comments](http://www.easyproject.cn/easycommons/en/index.jsp#donation 'Comments')

如果您有更好意见，建议或想法，请联系我。

If you have more comments, suggestions or ideas, please contact me.



Email：<inthinkcolor@gmail.com>

[http://www.easyproject.cn](http://www.easyproject.cn "EasyProject Home")



<img alt="支付宝钱包扫一扫捐助" src="http://www.easyproject.cn/images/s.png"  title="支付宝钱包扫一扫捐助"  height="256" width="256"></img>

<p>
<form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_blank">
<input type="hidden" name="cmd" value="_xclick">
<input type="hidden" name="business" value="inthinkcolor@gmail.com">
<input type="hidden" name="item_name" value="EasyProject development Donation">
<input type="hidden" name="no_note" value="1">
<input type="hidden" name="tax" value="0">
<input type="image" src="http://www.easyproject.cn/images/paypaldonation5.jpg"  title="PayPal donation"  border="0" name="submit" alt="Make payments with PayPal - it's fast, free and secure!">
</form>
</P>