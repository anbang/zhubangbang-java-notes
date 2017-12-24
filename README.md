** 朱邦邦的Java学习笔记 **

##### Java分为三个体系

- Java SE （也叫J2SE，Java 2 Platform Standard 	Edition，JAVA平台标准版，可以理解为JAVA桌面版本）
- Java EE （也叫J2EE，Java 2 Platform Enterprise Edition，JAVA平台企业版，用于构建大型的网站）
- JAVA ME （也叫J2ME，Java 2 Platform Micro		Edition，JAVA平台微型版，用户手机移动终端）


##### JAVA的开发环境

- Eclipse 比较流行
- Myeclipse 更适合我的
- IDEA
- Jbuilder
- Jdeveloper
- Netbeans
- JCreator


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

JRE，运行java程序所必须环境的集合，包含JVM标准实现及Jva核心类库，仅能够完成java的运行，而无法对java进行编译，调试等；JRE有独立版本，如果仅仅需要运行java程序，安装JRE即可；

** JDK **

JDK（java development kit） 是java语言的软件开发工具包（SDK），是面向java开发者发布的java套件；

JDK包含的基本组件包括：编译器，jar打包工具，javadoc文档生成器，debug调试器，头文件生成器，反汇编器、监控工具等；

JDK中包含完整的JRE，如果装了JDK，则不必再次安装JRE；


##### JAVA环境配置

- 安装编辑器 Eclipse / IDEA
	- https://www.eclipse.org/
- 安装JDK 
	- http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html


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


##### Eclipse的快捷键小结

- sysout或者syso 再加Alt + / 就可以输出 System.out.println("");

