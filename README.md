** 朱邦邦的Java学习笔记 **

##### 为什么学JAVA

为了以后回头看，不忘初衷，这里记录下；

**我碰到的困惑：**

目前是一个前端开发人员，做项目的时候，经常追着后端要接口，每当这个时候，我内心的真实想法是“不就是一些现有数据的输出汇总吗,怎么每次都好像要处理很多事情的样子”，其是用echarts做统计报表的时；我想每个前端对后端的工作都或多或少的这种感觉，只是有些人说出来，有些人不说出来罢了；（我个人只折腾过NODE，用Node写一些DEMO性质的接口，做中间件啥的，虽然知道后端很系统，很复杂，但是具体是哪些地方复杂，为了系统性需要注意哪些事情？都是没具体概念的；）

前端页面设计的时候，出发点是使用者的角度，而不是数据表结构的角度；后端看需求的时候，出发点可能是数据结构等周边方面；想多了解下数据结构方面的知识；而且因为工作需要和后端打交道的原因，其实我内心也是非常想探索一下后端的；

** 为什么是JAVA？ **

在前端里，JS是一等公民，所有的一切都是以HTML、CSS、JS为基础扩散出去的；

打算进入后端后，我碰到的第一个问题就是“选择什么语言进入后端”，后端语言给我的第一印象是像八国联军一样，c#/c++/java/php/python/go... 当然还有我们前端人最爱追NodeJS；

查了下企业语言，只有JAVA和C#这2个选择了，这个领域好像没有多少PHP、python、node的声音；又看了下语言的占比，JAVA一直第一名；

我的目的是选一门语言进入后端，选占有率最高的JAVA、相当于来说靠谱的概率更大一些；

题外话，本来是打算继续研究NODE的，就不往JAVA上研究了，但是无奈NODEJS的经典书籍真的太太太太少，因为官网node版本更新的太快，NODE的书籍确实很无奈，靠谱的基本就官方文档了，国内的NODE周边都是无脑吹前端进入后端最好的就是Nodejs，用NodeJS可以少学一门语法，JS写的可以前后端复用等等；尼玛无论青红皂都是这么强推，感觉真实太扯淡了，我学习的目的是想关心企业真实场景的后端相关，如果可以更好的与人沟通，多学一门语法又不是多费劲的事情,,，何必天天嘴上喊着要接受新事物，但实际上又总想着自己那一亩三分地呢,这些人都是圣母婊，，，，而且很多node的资源、视频、文章都是前端人，根据官网文档，或者自己工作一部分写的，糟粕太多，基本都是DEMO型的产品，根本没有系统性，，，好吧，我可能是个假前端。

---- 以上内容写在2017年12月25日(圣诞节)

### 写代码之前要思考的

- 明确真正需求；
	- 我真正要做的是什么东西？
- 分析思路
	- 我要分成第一步、第二步、第三步、xxx
- 确定步骤
	- 第一步我要做什么
	- 第二步我要做什么
	- ....
- 代码实现
	- 打开编辑器，具体的写；



##### Java分为三个体系 / 三种技术架构

- Java SE （也叫J2SE，Java 2 Platform Standard 	Edition，JAVA平台标准版，可以理解为JAVA桌面版本,其它两者基础）
- Java EE （也叫J2EE，Java 2 Platform Enterprise Edition，JAVA平台企业版，用于构建大型的网站）
- JAVA ME （也叫J2ME，Java 2 Platform Micro		Edition，JAVA平台微型版，用户手机移动终端）


##### JAVA的开发环境 / 编辑器

- Eclipse 比较流行
- IDEA (更适合我的,IDEA写前端代码还是很High的)


##### JAVA程序的运行环境

编写好的JAVA程序不能够直接在系统中运行，而是运行在JAVA虚拟机当中，Java虚拟机也称为JVM（Java Virtual Machine ），它是Java运行环境的一部分，Java运行环境又称为JRE（Java Runtime Environment）。

只要电脑中安装了JRE，就可以运行JAVA程序；


##### 如何开发JAVA

1.JAVA源代码是 xxxx.java 形式纯文本文件，可以使用任何文本编辑器编写，但不可执行；
2.JDK是JAVA语言的发开包，可以将第一步中 xxxx.java 文件编译为可执行的Java程序
	- 此时如果非开发环境下，可执行的java程序，是不能直接运行的；需要JVM才可以运行；
3.JRE包含了JVM、JDK中包含了JRE；
	- 如果仅仅需要运行java程序，安装JRE即可；
	- JDK是面向java开发者发布的java套件；


** JRE ** 

JRE；运行java程序所必须环境的集合，包含JVM标准实现及Jva核心类库，仅能够完成java的运行，而无法对java进行编译，调试等；JRE有独立版本，如果仅仅需要运行java程序，安装JRE即可；

JRE是Java程序的运行环境（Java运行的所需的类库+JVM/java虚拟机）

** JDK **

JDK是Java的开发和运行环境，java的开发工具和JRE。

JDK（java development kit） 是java语言的软件开发工具包（SDK），是面向java开发者发布的java套件；

JDK包含的基本组件包括：编译器，jar打包工具，javadoc文档生成器，debug调试器，头文件生成器，反汇编器、监控工具等；

JDK中包含完整的JRE，如果装了JDK，则不必再次安装JRE；


##### JAVA环境配置

- 安装编辑器 Eclipse / IDEA
	- https://www.eclipse.org/
- 安装JDK 
	- http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

注意：JDK安装，默认路径安装最好，如果更改安装路径需要手动配置环境变量的，类似装NODE配环境；


##### JAVA的编译和运行；

java是分两部分的：一个是编译，一个是运行。

就是javac命令和java命令；

- javac：
	- 负责的是编译的部分，当执行javac时，会启动java的编译器程序。对指定扩展名的.java文件进行编译。 生成了jvm可以识别的字节码文件。也就是class文件，也就是java的运行程序。
- java：
	- 负责运行的部分.会启动jvm.加载运行时所需的类库,并对class文件进行执行.

一个文件要被执行,必须要有一个执行的起始点,这个起始点就是main函数。

##### JAVA项目结构

- JRE System Library 
	- 系统运行时提供的环境和API
- src 开发的目录
	- com.zhubangbang.hello.main
		- Main.java
	- com.zhubangbang.hello.model
		- Model.java
	- com.zhubangbang.hello.view
		- View.java
- lib 资源目录

需要仔细整理和研究下项目结构

##### Eclipse的快捷键小结

- sysout或者syso 再加Alt + / 就可以输出 System.out.println("");

需要研究下Eclipse的常用快捷键

# JAVA的学习目录

** 编写Java程序时，应注意以下几点：**

- 大小写敏感：
	- Java是大小写敏感的，这就意味着标识符Hello与hello是不同的。
- 类名：
	- 对于所有的类来说，类名的首字母应该大写。如果类名由若干单词组成，那么每个单词的首字母应该大写，例如 MyFirstJavaClass 。
- 方法名：
	- 所有的方法名都应该以小写字母开头。如果方法名含有若干单词，则后面的每个单词首字母大写。
- 源文件名：
	- 源文件名必须和类名相同。当保存文件的时候，你应该使用类名作为文件名保存（切记Java是大小写敏感的），文件名的后缀为.java。（如果文件名和类名不相同则会导致编译错误）。
- 主方法入口：
	- 所有的Java 程序由public static void main(String []args)方法开始执行。


** 详细知识点 ** 

- 语法基础
- 对象和类
- 数据类型
- 变量类型
- 修饰符
- 运算符
- 循环语句 / 循环结构
- 判断语句 / 分支结构
- 类 Number
- 类 Math
- 类 Character
- String
- StringBuilder
- Array
- Date
- 正则
- Function
- Stream/File/IO
- Scanner
- 异常处理