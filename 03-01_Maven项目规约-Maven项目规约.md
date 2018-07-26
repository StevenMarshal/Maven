# 3 Maven项目规约

Maven项目目录：

* src/main/java
 
存放项目的.java 文件（开发源代码）

* src/main/resources

存放项目配置文件，如果没有配置文件该目录可无，如spring, hibernate 配置文件

* src/main/webapp

存放web 项目资源文件（web 项目才有）

* src/test/java

存放所有测试.java 文件（测试源代码）

* src/test/resources

测试配置文件，如果没有配置文件该目录可无target —— 项目输出位置（可无）

* pom.xml

maven 项目核心配置文件

也就是如果是一个Maven 项目那么它的根目录下必定存在src 文件夹和pom.xml。

pom.xml文件：

* project

任何要build 的事物，Maven 都认为它们是工程。这些工程被定义为工程对象模型（POM，Poject Object Model）。一个工程可以依赖其它工程，一个工程也可以由多个子工程构成。

* POM

pom(pom.xml)是Maven 的核心文件，它是指示Maven 如何工作的元数据文件，类似于Ant的build.xml文件。pom.xml文件位于每个工程的根目录下。

* Plug-in

Maven 是由插件组织的，它的每一个功能都由插件提供。插件提供goal，并根据在pom 中找到元数据去完成工作。
