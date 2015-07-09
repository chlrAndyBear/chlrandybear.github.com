---
layout: post
title: JAVA开发环境配置
description: 坚持就是胜利，量变引发质变。
key: Java,Eclipse
---

###需要的安装包

* JDK：不论版本，JAVA环境必需软件
* Eclipse：JAVA开发集成环境，环境配置好后，解压就能用，下载请下载Eclipse IDE for Java EE Developers

###安装JDK

* 这里我们以JDK1.7.0_45为例。

1.一路next，我们安装到C盘下的Java文件夹中，之后的jre也安装在这里，方便管理。
2.环境变量配置：右键“计算机”，点击属性，点击右方“高级系统设置”，在弹出的页面中选择“环境变量”。

<div class="box fn-clear">
	<img src="/images/java2.jpg" />
</div>

3.配置如下：

* 新建变量，变量名JAVA_HOME，变量值C:\Java\jdk1.7.0_45

<div class="box fn-clear">
	<img src="/images/java3.jpg" />
</div>

* 新建变量，变量名CLASSPATH(大小写无所谓)，变量值：.;%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar;(一定不要丢掉前面的点)(如果CLASSPATH存在，则修改，在变量值后面追加这部分代码，记得用分号分隔之前的代码)

<div class="box fn-clear">
	<img src="/images/java4.jpg" />
</div>

* 在变量Path中追加代码：%JAVA_HOME%\bin;%JAVA_HOME%\jre\bin;(记得用分号分隔之前的代码)。

运行cmd，输入java -version和javac指令，如果输出结果不是command not found则表示配置成功。

###Eclipse安装

下载好相应的Eclipse压缩包，解压到合适位置，运行eclipse.exe即可。
