# tomcat服务url访问服务器图片

先在服务器上配置tomcat

然后在tomcat/con/server.xml中加上
```xml
<Context path="/images" docBase="/home/rkayer/images"  reloadable="true"></Context>

```
path = "url访问时的路径" docbase = "服务器上文件存储的路径"

> $ systemctl daemon-reload

> $ systemctl restart tomcat

![](http://47.100.247.43:8080/images/amia.jpg)

