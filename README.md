很多时候打项目的时候会遇到jndi注入用不了ldap协议的情况，但是rmi却可以用，于是诞生了这个可能没什么用的工具。


适用于目标用不了ldap的情况

懒人专属，老规矩，富婆扫描器，不想努力就用它。不用自己写class打rmi了


# 用法：
把文件全上传到服务器/VPS上

## 先启动Log4jWeb-0.0.1：
```bash
java -jar Log4jWeb-0.0.1.jar
```

## 然后启动Log4j2Memory-0.1.jar
```bash
java -jar Log4j2Memory-0.1.jar
```
就可以食用


# 工具说明：
暂时只有三种类型可供选择：filter、Servlet、listener

目前暂时只支持注入部分基于tomcat8-10环境的内存马（部分springboot等）



后续会持续更新内存马

# 使用说明：

所有内存马参数都是chan，servlet的url是/p，如果参数是空会显示404

效果图(Log4j漏洞演示)：
![1656412703491851573876_62784214476_AA511B22-7E18-43e5-AA76-80E78536408D](https://user-images.githubusercontent.com/45167857/176162994-fa324ab7-a1ba-421a-abdd-2bc5934d3d18.png)

![1656412703489851573876_62784406554_C971527D-2BB6-4761-A2F6-DF67E5FA5CF6](https://user-images.githubusercontent.com/45167857/176163024-1dc03080-6435-4db7-b26d-00b5c9be275d.png)

![1656412703487851573876_62784295407_85A8F99C-24F3-491f-B56B-AD536D8D43FC](https://user-images.githubusercontent.com/45167857/176163039-bbe39fe6-dc64-4b43-8ec1-76faa37fbbc2.png)

内存马来自项目：https://github.com/ce-automne/TomcatMemShell

# 法律
```bash
本工具仅能在取得足够合法授权的企业安全建设中使用在使用,
本工具过程中，您应确保自己所有行为符合当地的法律法规。
如您在使用本工具的过程中存在任何非法行为，您将自行承担所有后果，本工具所有开发者和所有贡献者不承担任何法律及连带责任。
除非您已充分阅读、完全理解并接受本协议所有条款，否则，请您不要安装并使用本工具。
您的使用行为或者您以其他任何明示或者默示方式表示接受本协议的，即视为您已阅读并同意本协议的约束
```
