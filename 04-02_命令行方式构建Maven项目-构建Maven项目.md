## 4.2 构建Maven项目命令的使用

### 4.2.1 Maven常用命令

注：需要先进入项目目录后再操作！

|命令	|说明|
|-------|----|
|mvn clean 	|清除原来的编译结果|
|mvn compile 	|编译|
|mvn test 	|运行测试代码；mvn test -Dtest=类名//单独运行测试类|
|mvn package 	|打包项目；mvn package -Dmanven.test.skip=true//打包时不执行测试|
|mvn install 	|将项目打包并安装到本地仓库|
|mvn deploy 	|发布到本地仓库或者服务器|

4.2.2.	应用命令构建
构建需要在项目根目录下进行；首次使用maven 进行构建需要连网下载对应的各个命令插件。
运用mvn clean、mvn compile 。。。mvn install 进行构建。
