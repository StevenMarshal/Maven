## 2.2 settings.xml 配置文件

|节点名称	|说明|
|-----------|----|
|localRepository	|这个值是构建系统的本地仓库的路径。默认的值是${user.home}/.m2/repository.如果一个系统想让所有登陆的用户都用同一个本地仓库的话，这个值是极其有用的。|
|interactiveMode	|如果Maven 要试图与用户交互来得到输入就设置为true，否则就设置为false，默认为true。|
|offline	|如果构建系统要在离线模式下工作，设置为true，默认为false。如果构建服务器因为网络故障或者安全问题不能与远程仓库相连，那么这个设置是非常有用的。|
|pluginGroups	|当插件的组织Id（groupId）没有显式提供时，供搜寻插件组织Id（groupId）的列表。该元素包含一个pluginGroup元素列表，每个子元素包含了一个组织Id（groupId）。当我们使用某个插件，并且没有在命令行为其提供组织Id（groupId）的时候，Maven 就会使用该列表。默认情况下该列表包含了org.apache.maven.plugins。|
|proxies	|用来配置不同的代理，多代理profiles 可以应对笔记本或移动设备的工作环境：通过简单的设置profile id 就可以很容易的更换整个代理配置。|
|servers	|配置服务端的设置；一般用于设置安全认证等信息。一些设置如安全证书不应该和pom.xml 一起分发。这种类型的信息应该存在于构建服务器上的settings.xml 文件中。|
|mirrors	|镜像库。确定使用的仓库；为仓库列表配置的下载镜像列表。|
|profiles	|根据环境参数来调整构建配置；需要激活才能生效。|
|activeProfiles	|手动激活profiles 的列表【注意：必须与prifile 的id 一致】|
